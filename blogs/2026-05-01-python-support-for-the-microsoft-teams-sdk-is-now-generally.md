---
title: "Python support for the Microsoft Teams SDK is now generally available"
url: "https://devblogs.microsoft.com/microsoft365dev/python-support-for-the-microsoft-teams-sdk-is-now-generally-available/"
date: "Fri, 01 May 2026 20:15:16 +0000"
author: "Lily Du, Ricky Castaneda, Aamir Jawaid"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p><span>Today we’re announcing the general availability (GA) of </span><b><span>Python support in the Microsoft Teams SDK.</span></b><span> Python developers can now build Teams-native apps and agents using the same SDK surface that powers modern Teams experiences across our TypeScript and .NET stacks</span><span> </span></p>
<h2><b><span>Get started</span></b><span> </span></h2>
<p>In your terminal:</p>
<pre class="prettyprint language-default"><code class="language-default">pip install microsoft-teams-apps</code></pre>
<p>Basic usage:</p>
<pre class="prettyprint language-default"><code class="language-default">from microsoft_teams.apps import App, ActivityContext 
from microsoft_teams.api import MessageActivity 
 
app = App() 
 
@app.on_message 
async def handle_message(ctx: ActivityContext[MessageActivity]): 
   await ctx.send(f"You said: {ctx.activity.text}") 
 
# Start the app 
await app.start() </code></pre>
<p><span>With Python support, your orchestration logic, reasoning layer, workflow automation, or domain-specific agents can now:                                                                                              </span><span> </span></p>
<ul>
<li><span> Participate in chats, channels, and meetings as a first-class Teams app</span><span> </span></li>
<li><span> Stream responses and render adaptive cards in conversation</span><span> </span></li>
<li><span> Plug into your existing Python server, agent framework, or LLM stack</span><span> </span></li>
<li><span> Send proactive in-conversation messages to users and groups         </span><span> </span></li>
</ul>
<h2><b><span>What&#8217;s included                                                                             </span></b><span> </span></h2>
<p><span>The Python release ships with the capabilities developers need to move from prototype to production:</span><span> </span></p>
<ul>
<li><span>Decorator-based activity routing. Handle messages, mentions, and conversation events using familiar Python decorators — no boilerplate, no custom dispatchers.</span></li>
<li><span>Built-in OAuth. First-class user authentication flows are handled by the SDK, so you can focus on your app instead of token plumbing.</span><span> </span></li>
<li><span>Type-safe Microsoft Graph access. Call Microsoft Graph as the signed-in user or as the app via the <strong>user_graph</strong> and <strong>app_graph</strong> properties, with full type hints.</span><span> </span></li>
<li><span>Extensible plugin architecture. Compose middleware, telemetry, and custom behaviors into your app without modifying core SDK code.</span><span> </span></li>
</ul>
<h2><b><span>Start building today</span></b><span> </span></h2>
<p><span>With GA support for Python, developers have a direct path to extend their services into one of the most widely used collaboration platforms in the world.</span><span> </span></p>
<ul>
<li><b><span>Follow the quick start guide: </span></b><span>You can create a new Teams agent in seconds. The </span><a href="https://microsoft.github.io/teams-sdk/python/getting-started/">quick start</a> <span>guides you through it step by step.</span><span> </span></li>
</ul>
<ul>
<li><b><span>Explore an example: </span></b><span>Our </span><a href="https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/TeamsSDK/bot-quickstart/python/bot-quickstart"><span>Teams sample inventory</span></a><span> can help you dig deeper into the code to learn more via a hands-on experience. </span><span> </span></li>
</ul>
<ul>
<li><b><span>Join the community:</span></b><b><i><span> </span></i></b><span>Join the discussions in the Microsoft 365 Developer Forum, share your agent ideas or ask questions on Stack Overflow, and follow our updates on the Teams developer blog. Report any issues you experience in the <a href="http://aka.ms/NewIssue">Teams SDK repo</a>.</span></li>
</ul>
<p><span>We’re excited to see what you build!</span><span> </span></p>
<p><span>Learn more about the </span><a href="https://devblogs.microsoft.com/microsoft365dev/announcing-the-updated-teams-ai-library-and-mcp-support/"><span>Microsoft Teams SDK.</span></a><span> </span></p>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/python-support-for-the-microsoft-teams-sdk-is-now-generally-available/">Python support for the Microsoft Teams SDK is now generally available</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
