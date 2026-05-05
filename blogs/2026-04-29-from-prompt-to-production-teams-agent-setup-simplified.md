---
title: "From prompt to production: Teams agent setup, simplified"
url: "https://devblogs.microsoft.com/microsoft365dev/from-prompt-to-production-teams-agent-setup-simplified/"
date: "Wed, 29 Apr 2026 21:27:55 +0000"
author: "Aamir Jawaid, Umang Sehgal, Kavin Singh"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p dir="auto">You want to build a Teams agent. Maybe it answers customer questions from a knowledge base. Maybe it runs your team&#8217;s standups. The interesting part is the logic, the thing the agent actually <em>does</em>.</p>
<p dir="auto">But before you write a single line of that logic, you have to register it with Teams. That takes a number of steps.</p>
<div class="markdown-heading" dir="auto">
<h2 class="heading-element" dir="auto" tabindex="-1">How it works today</h2>
<p>Getting an agent into Teams requires configuring an identity, generating credentials, authoring a manifest, and wiring it all together. These steps span the Azure portal, Developer Portal, and your editor. Each one is straightforward on its own, but the context-switching between them adds up.</p>
</div>
<div dir="auto"><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/setup-steps.webp"><img alt="Image of the steps to add an agent to Teams." class="aligncenter wp-image-25610 size-medium" height="300" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/setup-steps-254x300.webp" width="254" /></a></div>
<div class="markdown-heading" dir="auto">
<h2 class="heading-element" dir="auto" tabindex="-1">Let your coding agent handle it</h2>
<p>The <a href="https://microsoft.github.io/teams-sdk/developer-tools/agent-skills"><code>teams-dev</code> agent skill</a> works with AI coding agents like Copilot, Claude Code, and Cursor. Instead of learning the registration steps yourself, tell your coding agent:</p>
</div>
<ul dir="auto">
<li><em>&#8220;Help me build a Teams agent that answers FAQs&#8221;</em></li>
<li><em>&#8220;Get my agent running in Teams&#8221;</em></li>
<li><em>&#8220;My agent isn&#8217;t loading in Teams, can you help?&#8221;</em></li>
</ul>
<p dir="auto"><a href="https://github.com/microsoft/teams-sdk/blob/main/teams.md/blog/2026-04-28-teams-cli-preview/agent-skill.gif" rel="noopener noreferrer" target="_blank"><img alt="The teams-dev agent skill in action" src="https://github.com/microsoft/teams-sdk/raw/main/teams.md/blog/2026-04-28-teams-cli-preview/agent-skill.gif" /></a></p>
<p dir="auto">The skill uses the CLI under the hood to handle the full infrastructure workflow, from sign in to a working agent in Teams, and troubleshooting when something breaks. Beyond infrastructure, it also helps your coding agent write application logic following best practices from the Teams SDK documentation.</p>
<div class="markdown-heading" dir="auto">
<h2 class="heading-element" dir="auto" tabindex="-1">Under the hood: The Teams CLI</h2>
<p>For developers who want direct control, the skill is powered by the next iteration of our CLI. Install it and sign in:</p>
</div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto">
<pre>npm install -g @microsoft/teams.cli@preview
teams login</pre>
<h3 class="zeroclipboard-container">Create is now just one command</h3>
</div>
<div class="markdown-heading" dir="auto">
<p><span style="font-family: Consolas, Monaco, monospace;">teams app create &#8211;name </span><span class="pl-s" style="font-family: Consolas, Monaco, monospace;"><span class="pl-pds">&#8220;</span>My Bot<span class="pl-pds">&#8220;</span></span><span style="font-family: Consolas, Monaco, monospace;"> &#8211;endpoint https://my-bot.example.com/api/messages &#8211;env .env</span></p>
</div>
<p dir="auto"><code>teams app create</code> does the heavy lifting (registration, credentials, manifest, and more) so you can start building immediately. All the steps from above happen behind the scenes.</p>
<p dir="auto"><a href="https://github.com/microsoft/teams-sdk/blob/main/teams.md/blog/2026-04-28-teams-cli-preview/app-create.gif" rel="noopener noreferrer" target="_blank"><img alt="Showcasing how a single command is able to set up your entire agent infra" src="https://github.com/microsoft/teams-sdk/raw/main/teams.md/blog/2026-04-28-teams-cli-preview/app-create.gif" /></a></p>
<p dir="auto">Now you can focus on your agent&#8217;s logic without worrying about app registration concepts. See the <a href="https://github.com/microsoft/teams-sdk/blob/main/cli">CLI docs</a> for all available flags.</p>
<div class="markdown-heading" dir="auto">
<h3 class="heading-element" dir="auto" tabindex="-1">Easy installation</h3>
<p>Traditionally, getting an agent into Teams means building an app package, managing a manifest, and sideloading it. With the CLI, <code>app create</code> gives you an installation link. Open it and Teams handles the install flow without a manual zip/package upload.</p>
</div>
<p dir="auto"><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/install-link.webp"><img alt="Screenshot of the My Bot agent." class="aligncenter wp-image-25612 size-medium" height="269" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/install-link-300x269.webp" width="300" /></a></p>
<p dir="auto">The CLI also includes a <code>teams app doctor</code> command that checks your agent&#8217;s registration, credentials, endpoint, and manifest so when something breaks, you know exactly what to fix.</p>
<p dir="auto">For CI pipelines and custom tooling, every CLI command supports <code>--json</code> output for programmatic consumption.</p>
<div class="markdown-heading" dir="auto">
<h2 class="heading-element" dir="auto" tabindex="-1">Get started</h2>
<p>Install the <code>teams-dev</code> agent skill (Copilot, Claude Code, Cursor):</p>
</div>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto">
<pre class="notranslate"><code>/plugin marketplace add microsoft/teams-sdk
/plugin install teams-sdk@teams-skills
</code></pre>
<div class="zeroclipboard-container">See the <a href="https://microsoft.github.io/teams-sdk/developer-tools/agent-skills/">agent skills guide</a> for VS Code and other editors.</div>
</div>
<p dir="auto">Install the CLI:</p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto">
<pre>npm install -g @microsoft/teams.cli@preview</pre>
<div class="zeroclipboard-container">For documentation, see <a href="https://microsoft.github.io/teams-sdk/cli/" rel="nofollow">microsoft.github.io/teams-sdk/cli</a>. To file issues, go to <a href="https://github.com/microsoft/teams-sdk/issues">github.com/microsoft/teams-sdk</a>.</div>
</div>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/from-prompt-to-production-teams-agent-setup-simplified/">From prompt to production: Teams agent setup, simplified</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
