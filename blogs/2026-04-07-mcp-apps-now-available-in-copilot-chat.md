---
title: "MCP Apps now available in Copilot chat"
url: "https://devblogs.microsoft.com/microsoft365dev/mcp-apps-now-available-in-copilot-chat/"
date: "Tue, 07 Apr 2026 20:56:49 +0000"
author: "Deepak Pratinidhi"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p>On March 9, <a href="https://techcommunity.microsoft.com/blog/microsoft365copilotblog/enable-agents-to-bring-apps-into-the-flow-of-work%E2%80%94while-keeping-it-in-control/4499464">Microsoft announced a major step forward in agent capabilities</a>: agents can now bring rich, app powered UI experiences directly into Microsoft 365 Copilot chat, via <a href="https://modelcontextprotocol.io/extensions/apps/overview">MCP Apps</a> or the <a href="https://developers.openai.com/apps-sdk">OpenAI Apps SDK</a>. Both work seamlessly with Copilot.</p>
<h2>From conversational to interactive</h2>
<p>Traditional apps are evolving with the help of intelligent agents that do more than deliver information—they help users take action in those apps directly from Copilot chat, with built in control and transparency. Through interactive, HTML based interfaces, agents can surface relevant data and next steps without forcing users to switch apps or lose conversational context, all grounded in organizational insights from Work IQ.</p>
<p>Using MCP Apps or the Apps SDK, agents go well beyond text responses. They can present tables, forms, diagrams, dashboards, maps, rich media, and specialized creation surfaces, all securely rendered in a sandboxed iFrame within chat. Agents can then guide users through next steps, request input when needed, and carry out instructions on their behalf.</p>
<p>Together, <a href="https://techcommunity.microsoft.com/blog/microsoft365copilotblog/a-closer-look-at-work-iq/4499789">Work IQ</a> and apps in agents enable powerful end to end workflows for developers and organizations. Work IQ supplies the context—helping Copilot understand meetings, emails, and organizational data. For example, Copilot can automatically match travel receipts from email, update a CRM opportunity after a meeting, or reconcile invoices. With app powered UI rendered inline or side by side in chat, structured data like forms and tables appears exactly where users need it, turning complex workflows into seamless experiences.</p>
<h2>What customers and partners are building</h2>
<p>Here are a few examples of how Microsoft partners have used MCP Apps and Apps SDK to build interactive, in-chat app experiences for Copilot:</p>
<h3><strong>Data entry and visualizations</strong></h3>
<p>Need to automate data entry based on information available in Work IQ, or view information in a richer format like a heat map? <a href="https://www.microsoft.com/en-us/power-platform/blog/power-apps/public-preview-your-business-apps-now-part-of-every-conversation/">Power Apps agents</a> bring all these capabilities to chat with compelling visualizations.</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/AppSkillsInBizChat.gif"><img alt="AppSkillsInBizChat example GIF" class="size-full wp-image-25510 alignnone" height="1028" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/AppSkillsInBizChat.gif" width="1908" /></a></p>
<h3>Project or process management</h3>
<p>Bring records from enterprise or partner applications directly into Copilot with added context from Work IQ. This example from Microsoft Expense illustrates automatically matching and attaching expense receipts from emails to pending credit card transactions for streamlined expense reporting.</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/MS_Expense_v3-3_resized.gif"><img alt="MS Expense GIF animation" class="size-full wp-image-25570 alignnone" height="1150" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/MS_Expense_v3-3_resized.gif" width="2048" /></a></p>
<p>&nbsp;</p>
<h3>Content generation</h3>
<p>Whether it’s building marketing flyers and social assets in Adobe Express, structured FigJam diagrams in Figma, or graphic designs in Canva, apps in agents lets users design the whole project in natural language. For example, Figma can help generate an employee onboarding workflow customized to a user’s instructions in chat.</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/Figma_Updated-1.gif"><img alt="FigJam example GIF" class="size-full wp-image-25513 alignnone" height="2160" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/Figma_Updated-1.gif" width="3840" /></a></p>
<h3>Employee training and learning resources</h3>
<p>Curious to learn more about a new technology you just heard about in a meeting? Simply prompt Copilot to explore learning tools and resources on Coursera- directly alongside the tasks you&#8217;re already working on:</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/Coursera-launches-the-first-learning-agent-in-Microsoft-365-Copilot-enabled-by-Apps-SDK-1.gif"><img alt="Coursera launches the first learning agent in Microsoft 365 Copilot enabled by Apps SDK 1 image" class="size-full wp-image-25527 alignnone" height="453" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/Coursera-launches-the-first-learning-agent-in-Microsoft-365-Copilot-enabled-by-Apps-SDK-1.gif" width="800" /></a></p>
<p>&#8220;Bringing the monday.com experience into the environments our customers already depend on is a natural evolution of how work gets done,” said Shanee Radzewsky, monday.com&#8217;s API &amp; MCP Team Lead. “With MCP Apps, we&#8217;re meeting teams where work already happens and extending <a href="https://nam06.safelinks.protection.outlook.com/?url=http%3A%2F%2Fmonday.com%2F&amp;data=05%7C02%7CStephanie.Hass%40microsoft.com%7Cd86549c8214549c1e57508de918f3cea%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C639108241546722999%7CUnknown%7CTWFpbGZsb3d8eyJFbXB0eU1hcGkiOnRydWUsIlYiOiIwLjAuMDAwMCIsIlAiOiJXaW4zMiIsIkFOIjoiTWFpbCIsIldUIjoyfQ%3D%3D%7C0%7C%7C%7C&amp;sdata=YKro%2FHernI8YvtVgzkGrIyJq2tVmmLT3xVP9bmHdk0U%3D&amp;reserved=0">monday.com</a> into the tools they use every day, helping turn context into action and move work forward faster with AI.”</p>
<p><span>You can try apps in agents with our launch partners, including Outlook (compose and scheduling), Power Apps (available now in public preview), Adobe Express (available now), Coursera (available now), Figma (available now), monday.com (available now), and more. All pre-built partner app experiences will be available via the <a class="fui-Link ___1q1shib f2hkw1w f3rmtva f1ewtqcl fyind8e f1k6fduh f1w7gpdv fk6fouc fjoy568 figsok6 f1s184ao f1mk8lai fnbmjn9 f1o700av f13mvf36 f1cmlufx f9n3di6 f1ids18y f1tx3yz7 f1deo86v f1eh06m1 f1iescvh fhgqx19 f1olyrje f1p93eir f1nev41a f1h8hb77 f1lqvz6u f10aw75t fsle3fq f17ae5zn" href="https://m365.cloud.microsoft/chat/agentstore/" id="menurj2u" rel="noreferrer noopener" target="_blank" title="https://m365.cloud.microsoft/chat/agentstore/">Microsoft 365 Agent Store</a> by mid-April. Simply select an agent in Copilot chat or @mention it to get started.</span></p>
<h2>Getting started</h2>
<p>Ready to build your own agent? <a href="https://modelcontextprotocol.io/docs/learn/server-concepts">MCP servers</a> offer a consistent, secure, and low-friction way for AI models to access the tools and resources they need. Your current functionality, authentication, and integrations stay intact. UI components are layered through the meta property, ensuring they’re additive and backward compatible. That means your app continues to work seamlessly across existing clients—while gaining new interactive capabilities in Copilot.</p>
<p>If you are building a new MCP server, <a href="https://modelcontextprotocol.io/docs/develop/build-server">MCP official SDKs</a> are the fastest way to get started. Once your MCP server is in place, there are two straightforward ways to integrate it:</p>
<ol>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/declarative-agent-ui-widgets">Use the Microsoft 365 Agents Toolkit</a> for Visual Studio Code. In VS Code, select “Add an Action,” choose “Start with an MCP Server,” and then provide the URL for your MCP server (using either MCP Apps or the Apps SDK for UI components).
<a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/DevX-1.gif"><img alt="DevX 1 image" class="alignleft size-full wp-image-25594" height="1654" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/DevX-1.gif" width="2490" /></a></li>
<li>Use the <a href="https://github.com/microsoft/work-iq">GitHub Copilot CLI skill</a> for Microsoft 365 Agents Toolkit. This lets you go from zero to a fully deployed Copilot agent — complete with an MCP server, authentication and rich interactive widgets — in a single conversation with an AI agent. Our composable skills handle the entire lifecycle: scaffolding, MCP server development, authentication setup, widget rendering, tool discovery, and deployment. The AI agent does heavy lifting. You describe what you want in natural language. For example:</li>
</ol>
<pre class="prettyprint language-default"><code class="language-default"># Install the plugin
/plugin marketplace add microsoft/work-iq
/plugin install microsoft-365-agents-toolkit@work-iq#

Then just ask
"Create a declarative agent that uses an MCP server with a dashboard widget for my insurance claims"</code></pre>
<p><a href="https://www.youtube.com/watch?v=m106AA3khJI"><img alt="video thumbnail image" class="alignnone wp-image-25544 size-full" height="214" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/video-thumbnail.webp" width="384" /></a></p>
<p>The platform supports OAuth 2.1, <a href="https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/what-is-single-sign-on">Microsoft Entra single sign-on (SSO)</a>, and anonymous authentication. Agents that include interactive app experiences follow the same governance, security, and administrative controls as other declarative agents used across your organization.</p>
<p>Questions while building? Check out our developer resources at the bottom to connect with us!</p>
<h2>UX considerations</h2>
<p>When designing agents, follow established <a href="https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/declarative-agent-ui-widgets-guidelines">UX best practices</a> and prioritize natural language interactions. In Microsoft 365 Copilot, apps can be surfaced in two complementary ways, depending on the complexity of the experience you’re delivering:</p>
<ol>
<li><strong>Inline mode (required)</strong> displays lightweight widgets directly in the conversation, appearing before the model’s generated response. This is the default Copilot surface and is ideal for quick interactions such as document previews, simple actions, decision prompts, or confirmations.</li>
<li>For more advanced scenarios, <strong>side by side mode (optional)</strong> provides an expanded, immersive workspace alongside the conversation. This layout is designed for richer workflows that are difficult to deliver inline, including multistep editing, complex visual layouts, and extended review or comparison tasks.</li>
</ol>
<h2>Quick start samples</h2>
<p>Want to move even faster? Use official <a href="https://github.com/modelcontextprotocol/ext-apps">MCP Apps samples</a> or <a href="https://github.com/openai/openai-apps-sdk-examples">Apps SDK samples</a> or to get started or try out the samples below.</p>
<ol>
<li><strong>Field Service Dispatch</strong>: MCP server for a field service dispatch workflow with assignment intake, map visualization, dispatch planning, and confirmation flow. Requires a free Mapbox token for map widgets.
<ol type="a">
<li><a href="https://github.com/microsoft/mcp-interactiveUI-samples/blob/main/mcp-apps/fieldops/node/src/mcpserver/README.md">MCP Apps version</a></li>
<li><a href="https://github.com/microsoft/mcp-interactiveUI-samples/blob/main/oai-apps-sdk/fieldops/node/README.md">Apps SDK version</a></li>
</ol>
</li>
<li><strong>Trey Research — HR Consultant Managemen</strong>t: MCP server for managing HR consultants, projects, and assignments with Fluent UI React widgets including an HR dashboard, consultant profile cards, bulk editor, and project detail views.
<ol type="a">
<li><a href="https://github.com/microsoft/mcp-interactiveUI-samples/blob/main/mcp-apps/trey-research/node/src/mcpserver/README.md">MCP Server using MCP Apps</a></li>
<li><a href="https://github.com/microsoft/mcp-interactiveUI-samples/blob/main/oai-apps-sdk/trey-research/node/src/mcpserver/README.md">MCP Server using Apps SDK</a></li>
</ol>
</li>
<li><strong>Employee Training</strong>: MCP server that recommends learning and training courses with embedded video previews, inline entity cards, and full-screen course views.
<ol type="a">
<li><a href="https://github.com/microsoft/mcp-interactiveUI-samples/blob/main/mcp-apps/employee-training/node/README.md">MCP Apps version</a></li>
</ol>
</li>
</ol>
<p>Check out all of our samples in the <a href="https://github.com/microsoft/mcp-interactiveUI-samples?tab=readme-ov-file">mcp-interactiveUI-samples repo</a> on GitHub.</p>
<h2>Publish for your organization or the public agent store</h2>
<p>You can use these tools to build agents for yourself, your team or organization, or publish to the <a href="https://m365.cloud.microsoft/chat/agentstore/?fromCode=CsrToSSR&amp;auth=2">Microsoft 365 Agent Store</a> for easy discovery across Copilot and Microsoft 365 apps. Here is more information on sharing for quick testing, publishing to your organization, or publishing at scale.</p>
<ol>
<li><a href="https://learn.microsoft.com/en-us/copilot/microsoft-365/agent-essentials/agent-policies/agent-sideload">Sideload agents</a> to share within your organization without going through publishing for quick testing. Usually limited for developer.</li>
<li>To share and <a href="https://learn.microsoft.com/en-us/microsoft-365/admin/manage/manage-copilot-agents-integrated-apps">manage declarative agents</a> internally with your team or organization, you can deploy agents through the Microsoft 365 Admin Center. Once an IT administrator approves the agent, it appears in the Agent Store and can be scoped to specific users or groups based on organizational policies.</li>
<li>For partners and developers who want to reach customers at scale, you can publish agents to the Microsoft 365 Agent Store for discovery across tenants. Review the <a href="https://github.com/MicrosoftDocs/m365copilot-docs/blob/main/docs/publish.md">submission guidelines</a> to learn more. Once Microsoft validates and approves your app package, your agent becomes available in the Microsoft Commercial Marketplace and is ready for IT enablement. After an IT administrator enables an agent built by your team, partners, or third-parties, it appears in the Agent Store and other Microsoft 365 apps such as Teams, Outlook, Word, Excel, and PowerPoint.</li>
</ol>
<h2>Engage with the developer community</h2>
<p>Building with MCP Apps or the Apps SDK and have questions? Join our developer communities to get support. We’re here to help you solve problems and keep your momentum going strong.</p>
<ol>
<li>Add your queries to Microsoft Q&amp;A here: <a href="https://learn.microsoft.com/en-us/answers/tags/466/microsoft-copilot-microsoft-365-copilot-development-routing">Microsoft Copilot | Microsoft 365 Copilot | Development</a></li>
<li>Head to GitHub repositories <a href="https://github.com/OfficeDev/microsoft-365-agents-toolkit">M365 Agents Toolkit</a> or <a href="https://github.com/microsoft/mcp-interactiveUI-samples">InteractiveUI samples</a></li>
<li>Engage in the <a href="https://www.reddit.com/r/copilotstudio/">copilotstudio</a> or <a href="https://www.reddit.com/r/microsoft_365_copilot/">microsoft_365_copilot</a> subreddits</li>
</ol>
<p>We can’t wait to see what you build!</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/mcp-apps-now-available-in-copilot-chat/">MCP Apps now available in Copilot chat</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
