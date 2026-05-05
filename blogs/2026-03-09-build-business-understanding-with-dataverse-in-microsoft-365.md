---
title: "Build business understanding with Dataverse in Microsoft 365 Copilot"
url: "https://devblogs.microsoft.com/microsoft365dev/build-business-understanding-with-dataverse-in-microsoft-365-copilot/"
date: "Mon, 09 Mar 2026 12:45:27 +0000"
author: "James Oleinik"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p><span>Business applications hold some of the most valuable data in an organization—customer’s financial records, sales pipeline, support cases, inventory orders—but that data has traditionally been locked behind app-specific experiences. Users switch between Dynamics 365, Power Apps, Outlook, and Teams to piece together the full picture. What if Copilot could understand your business data the way your best people do?</span><span> </span></p>
<h2><span>Microsoft 365 Copilot in business apps</span><span> </span></h2>
<p><span>Microsoft 365 Copilot is now embedded as an in-app sidecar within Power Apps, Dynamics 365 Sales, and Dynamics 365 Customer Service—removing the need to switch between apps to find context or complete steps.</span><span> </span></p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/Dataverse-and-M365-Copilot.webp"><img alt="An image showing Dataverse within Microsoft 365 Copilot." class="alignnone size-large wp-image-25391" height="562" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/Dataverse-and-M365-Copilot-1024x562.webp" width="1024" /></a></p>
<p>&nbsp;</p>
<p><b><span>Work IQ </span></b><span>is the reasoning layer, reconciling enterprise data and work signals from across your apps. Under the hood, Work IQ powers the combination of critical sources of business data and insights: Microsoft 365 apps, Dynamics 365 apps, and Power Platform. </span><span> </span></p>
<ul>
<li><b><span>Microsoft 365 data. </span></b><span> Emails, meetings, and documents from Microsoft 365 apps to deliver grounded, contextual answers.</span><span> </span></li>
</ul>
<ul>
<li><b><span>Dynamics 365 and Power Platform data. </span></b><span>Relevant business records (accounts, opportunities, leads, activities, and your custom entities) from Dataverse.</span><span> </span></li>
</ul>
<h2><span>What&#8217;s New: Intelligent semantic layer for business understanding</span><span> </span></h2>
<p><span>By leveraging </span><a href="https://www.microsoft.com/en-us/dynamics-365/blog/it-professional/2025/12/08/agentic-ai-dataverse-search/"><span>recent breakthroughs in Dataverse Agentic AI powered Dataverse Search</span></a><span>, Microsoft 365 Copilot within “in app” experiences (Power Apps, Dynamics 365 Sales, Dynamics 365 Service) delivers answers using an adaptive reasoning process based on schema and keywords (similar to how business logic retrieves records today). </span><span> </span></p>
<p><span>With this update, we are announcing that Dataverse Search is enriched with an </span><b><span>intelligent semantic layer</span></b><span> that understands the business data schema and adds true business data understanding for agents to operate. </span><span> </span></p>
<h2><span>What&#8217;s New: Capture hidden procedural knowledge as business understanding </span><span> </span></h2>
<p><span>Business understanding also enables organizations to </span><b><span>capture procedural knowledge</span></b><span> </span><b><span>from existing business workflows</span></b><span> as context to further inform Copilot. For example, as the sales lead, I need to draft a sales proposal to a customer. Before I start drafting an email, I need to: </span><span> </span></p>
<ul>
<li><b><span>Research</span></b><span>: Understand customer contact’s role on LinkedIn, review CRM records for recent conversations, and use messaging based on the latest sales play, and share any marketing promotions. </span><span> </span></li>
</ul>
<ul>
<li><b><span>Reviews</span></b><span>: Because this is a key account with existing contracts in place, I check with leadership to get their buy in. </span><span> </span></li>
</ul>
<ul>
<li><b><span>Optimize Readability</span></b><span>: Shorten the message so that it is mobile optimized.</span><span> </span></li>
</ul>
<p><span>Business understanding captures this hidden procedural knowledge and dynamically loads these instructions to answer relevant sales questions so that Copilot can perform domain specific tasks at the level of any expert (in this case the sales lead).</span><span> </span></p>
<h2><span>Seeing it in action</span><span> </span></h2>
<p><span>Previously, in Microsoft 365 Copilot, asking </span><i><span>&#8220;Help me understand which products are affected by pricing changes and identify my corresponding opportunities that are impacted by this change”</span></i><span> would not return a list of records because Copilot didn’t have your Dataverse context. </span><b><span>With business understanding</span></b><span>, the same question produces a precise list based on grounded data —no report building, no app switching, no guesswork. </span><span> </span></p>
<p><video controls="controls" height="150" width="300"><source src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/MSFT-2743-D365_Blog_Work_IQ.mp4" type="video/mp4" /></video></p>
<p><b><span>How was this accomplished?</span></b><span> With business understanding, Work IQ can now connect the dots, understand your business data, and know how to use it effectively. Without leaving Dynamics 365 Sales, Copilot understood that “ZavaCore Fiber – Nano Grade” and “ZavaCore Fiber – System Grade” were the affected products based on signals from Outlook messages. It then compared with the CRM records to find opportunities aligned to those impacted products: </span><span> </span></p>
<ul>
<li><span>“ZavaCore Fiber – NanoGrade” and “ZavaCore Fiber – System Grade” are product records in Dataverse and tagged in related opportunities.</span><span> </span></li>
</ul>
<ul>
<li><span>When users ask questions about finding an opportunity, Copilot knows to only analyze “open opportunities.&#8221; </span><span> </span></li>
</ul>
<h2><span>Activating business understanding with Dataverse MCP</span><span> </span></h2>
<p><span>Agents are only as smart as the data they can reach. Whether you&#8217;re building an agent in Copilot Studio, GitHub Copilot, or Azure AI Foundry, the quality of your agent&#8217;s responses depends entirely on its ability to find, understand, and reason over your business data. That&#8217;s where the Dataverse MCP server comes in.</span><span> </span></p>
<p></p>
<p><span>The </span><b><span>Dataverse Model Context Protocol (MCP) server</span></b><span> gives agents a structured, secure way to interact with your business data — inserting or updating records, reading from tables, searching knowledge, and executing prompts — all from within the agent&#8217;s context. Instead of building custom connectors, developers can point any MCP-compatible agent to Dataverse MCP and get instant access to rich, governed business data.</span><span> </span></p>
<p><span>Starting in late March, we&#8217;re enhancing the Dataverse MCP with new tools specifically designed to build </span><b><span>business understanding</span></b><span> for agents. Try them out on the Dataverse MCP preview endpoint:</span><span> <a href="https://aka.ms/dataversemcppreview">aka.ms/dataversemcppreview</a>.</span><span> </span></p>
<p><span>Dataverse MCP is available today across:</span><span> </span></p>
<ul>
<li><span>Microsoft Copilot Studio</span><span> </span></li>
</ul>
<ul>
<li><span>Azure AI Foundry</span><span> </span></li>
</ul>
<ul>
<li><span>GitHub Copilot</span><span> </span></li>
</ul>
<ul>
<li><span>Any MCP-compatible platform or agent runtime</span><span> </span></li>
</ul>
<p><span>Work IQ with business understanding</span><b><span> </span></b><span>means:</span><span> </span></p>
<ul>
<li><span>Dataverse Search now understands your data, not just your schema.</span><span> </span></li>
</ul>
<ul>
<li><span>Organizations can capture procedural knowledge from business workflows.</span><span> </span></li>
</ul>
<ul>
<li><span>Agent developers can use Dataverse MCP to access new tools that enable business understanding.</span><span> </span></li>
</ul>
<p><span>The result: business-aware answers grounded in real records and real work — without leaving your workflow. This is the platform that moves Copilot from organizational context to true business understanding.</span><span> </span></p>
<h2>Learn more</h2>
<ul>
<li><span><a href="https://aka.ms/D365BlogMarch9">What&#8217;s new in Dynamics 365</a></span></li>
</ul>
<ul>
<li><a href="https://www.microsoft.com/en-us/dynamics-365/blog/it-professional/2025/12/08/agentic-ai-dataverse-search/"><span>Agentic AI Dataverse Search</span></a></li>
</ul>
<ul>
<li><a href="https://www.microsoft.com/en-us/power-platform/blog/power-apps/whats-new-in-power-platform-february-2026-feature-update/"><span>What’s new in Power Platform: February 2026 feature update &#8211; Microsoft Power Platform Blog</span></a><span> </span></li>
</ul>
<ul>
<li><a href="https://learn.microsoft.com/en-us/power-apps/maker/data-platform/data-platform-intro"><span>What is Microsoft Dataverse? &#8211; Power Apps | Microsoft Learn</span></a><span> </span></li>
</ul>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/build-business-understanding-with-dataverse-in-microsoft-365-copilot/">Build business understanding with Dataverse in Microsoft 365 Copilot</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
