---
title: "SharePoint Framework (SPFx) roadmap update – April 2026"
url: "https://devblogs.microsoft.com/microsoft365dev/sharepoint-framework-spfx-roadmap-update-april-2026/"
date: "Tue, 28 Apr 2026 17:13:17 +0000"
author: "Vesa Juvonen"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p><strong>April continues the strong momentum for the <a href="https://aka.ms/spfx">SharePoint Framework</a> and the broader Microsoft 365 extensibility ecosystem.</strong> Over the past month, we have been making steady progress across the SPFx roadmap, refining delivery plans, connecting with the community in person, and preparing the next wave of platform updates. As always, our focus remains on <strong>quality, predictability, and enabling real-world scenarios</strong> for customers, partners, and developers building solutions at scale.</p>
<div>
<p>As part of our <strong>roadmap updates</strong> this month, we have aligned on a few changes to upcoming delivery plans to ensure we strike the <strong>right balance between innovation and enterprise readiness</strong>. One particularly exciting area of progress is a new AI-focused capability that is actively taking shape. While we are not ready to share full details yet, this upcoming feature is designed to help developers build more intelligent and assistive experiences as part of their SharePoint and Microsoft 365 solutions, and it is currently planned to <strong>head into public preview with the SPFx 1.24 release</strong>. We will have much more to share soon.</p>
<p>At the same time, we are approaching an important milestone with <strong>SPFx 1.23</strong>, which is on release candidate status. This release was a bit delayed from our initial plans as we wanted to ensure that right quality and to address any npm reported vulnerabilities. This release continues to focus on platform stability, refinements, and readiness, ensuring a solid foundation both for existing solutions and for the innovations coming next. If you have been following the previews, now is a great time to validate your solutions and prepare for the upcoming release.</p>
<p>April was also a <strong>great month for community connection</strong>. The <a href="https://m365conf.com">Microsoft 365 Community Conference</a> brought together developers, partners, and customers from around the world for deep technical sessions, practical learnings, and real-world stories. Conversations around SharePoint Framework, Microsoft 365 extensibility, and AI-driven scenarios reinforced the importance of building solutions that are grounded in real customer needs, while also looking ahead to what is possible next.</p>
<p>Looking forward, the next opportunity to continue these conversations is just around the corner at the <a href="https://collabsummit.eu/">European Collaboration Summit</a> (May 5-7). This event remains a <strong>key gathering for the SharePoint and Microsoft 365 community in Europe</strong>, with a strong focus on practical scenarios, learning, and connection. We are looking forward to meeting many of you there and continuing to shape the future of SPFx together.</p>
<div>
<h2>Release of SPFx v 1.23 release candidate</h2>
<div>
<p>We released already the latest release candidate for 1.23 with following new features. If you have the option, please test out things and provide us feedback on them.</p>
<ul>
<li>Grouping support for list view command sets</li>
<li>Preview of new <a href="https://aka.ms/spfx/cli">SPFx CLI</a> and open-sourced templates</li>
<li>Addressing npm audit issues</li>
</ul>
</div>
</div>
<p>See details on the 1.23 release on the release notes:</p>
<ul>
<li><a href="https://learn.microsoft.com/en-us/sharepoint/dev/spfx/release-1.23">SharePoint Framework 1.23 release candidate release notes</a></li>
</ul>
<p>We are currently looking into providing general availability (GA) of 1.23 in early May.</p>
<h2 id="roadmap">Roadmap</h2>
<p>We are evolving towards a quarterly release cycle, providing more predictability on new feature introductions and updates. We will update the <a href="https://learn.microsoft.com/en-us/sharepoint/dev/spfx/roadmap" rel="noopener" target="_blank">public roadmap</a> with any schedule and feature updates as we move forward in this journey.</p>
<p>Here is the set of investments which we are planning to ship within the upcoming SPFx releases:</p>
<h3 id="version-1.23-–-february/march-2026"><strong>Version 1.23 &#8211; May 2026</strong></h3>
<p>This release focuses on open sourcing the templates and tooling to create SPFx solutions, enabling our ecosystem to optionally build their own templates. We also want to focus on providing additional value for optimizing developer experience and providing new extensibility options.</p>
<ul>
<li><strong>Command set improvements</strong> for lists and libraries – grouping and potentially other improvements.</li>
<li>A new open-sourced <strong>SPFx CLI</strong> for replacing the existing Yeoman generator as <strong>preview release</strong> &#8211; You will be able to introduce your company specific templates or adjustments on the scaffolded baseline for the SPFx solutions. We are decoupling the CLI itself from the SPFx release versions.</li>
<li><b>Open-source </b><b>SPFx solution templates to GitHub</b> (when SPFx CLI is used)</li>
<li><b>New and edit panel override support</b> for lists and libraries</li>
<li>Other technical updates (eslint update)</li>
<li>Addressing any new npm audit vulnerability issues</li>
</ul>
<h3 id="version-1.24-–-may/june-2026"><strong>Version 1.24 &#8211; June 2026</strong></h3>
<p>This version continues providing new extensibility options aligned with the future direction of SharePoint. We are also expecting to have other new features and capabilities as part of this release, which will be disclosed a bit later.</p>
<ul>
<li><strong>Feature X  to public preview</strong> (disclosed soon)</li>
<li>Addressing any new npm audit vulnerability issues</li>
</ul>
</div>
<h3 id="version-1.24-–-may/june-2026"><strong>Version 1.25 &#8211; September 2026</strong></h3>
<p>This version continues providing new extensibility options aligned with the future direction of SharePoint. We are also expecting to have other new features and capabilities as part of this release, which will be disclosed a bit later.</p>
<ul>
<li><strong>Feature X  to general availability </strong>(disclosed soon)</li>
<li><strong>Navigation customizers</strong> – Options to override navigation nodes and/or experiences with SPFx components.</li>
<li><strong>SPFx CLI</strong> general availability (GA)</li>
<li>Last version of updated SPFx Yeoman generator &#8211; SPFx CLI will take over the scaffolding after this release</li>
</ul>
<h3>In top of mind</h3>
<p>These are features which are in top of our mind and we want to get them addressed as soon as possible.</p>
<ul>
<li><strong>React 18</strong> support for SPFx solutions &#8211; In previous communications, our estimate was that this is coming in June 2026. There&#8217;s work being actively done on updating the out-of-the-box web parts to the React 18 level. We can only enable it for custom web parts until that work is completed. This might happen by June, but we cannot currently confirm the schedule and are waiting for updates internally.</li>
</ul>
<div>
<p><strong>We also continue further innovation in the AI space</strong> with a focus on both customer features and developer tooling. More on this in future roadmap updates during 2026.</p>
<p>We encourage you to continue <strong>providing feedback to support our product planning for the upcoming semesters</strong>. We already have an extensive list of ideas and enhancements in mind but are always interested in your input.</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/sofx-roadmap-april-blog-roadmap.webp"><img alt="sofx roadmap april blog roadmap image" class="alignnone size-large wp-image-25602" height="576" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/04/sofx-roadmap-april-blog-roadmap-1024x576.webp" width="1024" /></a></p>
<h2 id="what’s-next">What’s next?</h2>
<p>We continue expanding the SharePoint platform to unlock more innovation across Microsoft 365:</p>
<ul>
<li><strong>SharePoint Framework (SPFx)</strong> for building rich, AI powered and business integrated solutions with custom user interfaces directly in Microsoft 365.</li>
<li><strong>SharePoint Embedded</strong> to bring SharePoint content into your own apps hosted outside of Microsoft 365 with your own user interface.</li>
<li><strong>Agents and AI</strong> to create intelligent, adaptive experiences to access your content and business information efficiently and expose those easily for your end users.</li>
<li><strong>Microsoft Graph</strong> to access data and insights everywhere using our standard API surface.</li>
</ul>
<p>We encourage you to explore these capabilities and see how they can help you build the next generation of solutions for your organization and customers.</p>
<div>
<p>If you are planning to build experiences for Microsoft 365, <strong>we strongly recommend joining our community calls</strong> and the broader <a href="https://aka.ms/community/home" rel="noopener" target="_blank">Microsoft 365 and Power Platform Community</a> activities. These cover Microsoft 365 Copilot, Power Platform, SharePoint, Microsoft Teams, Copilot Studio, Microsoft Graph, Microsoft Viva, and more. You can find call details and community assets at <a href="https://aka.ms/community/home" rel="noopener" target="_blank">https://aka.ms/community/home</a>.</p>
<p>You might also be interested in our <a href="https://www.youtube.com/watch?v=BNskpI7UctI&amp;list=PLR9nK3mnD-OUQ05Nos_l03oxBOeTsRGK4" rel="noopener" target="_blank">SharePoint partner showcase series</a> where we <strong>highlight solutions built with SharePoint</strong>. Each episode includes a video and a blog post with additional details. If you are creating something with SharePoint and would like to be featured, you can let us know by <a href="https://aka.ms/sharepoint/partner/showcase" rel="noopener" target="_blank">signing up through the provided form</a> and we will contact you to schedule a recording.</p>
<p>We are looking forward on having discussions with you all at the <a href="https://collabsummit.eu/">European Collaboration Summit 2026</a>. Hoping to see you all there.</p>
<p>Follow us also on <a href="https://www.linkedin.com/showcase/microsoft365dev/" rel="noopener" target="_blank">LinkedIn</a> or in <a href="https://x.com/microsoft365dev" rel="noopener" target="_blank">X</a> to stay up to date on Microsoft 365 Platform announcements.</p>
<p>Got feedback or input on this blog post &#8211; leave a comment and we will get back to you <img alt="&#x1f64b;&#x200d;&#x2642;" class="emoji" draggable="false" src="https://s.w.org/images/core/emoji/17.0.2/svg/1f64b-200d-2642-fe0f.svg" /></p>
<p>Happy coding! <strong>Sharing is Caring!</strong> <a class="lightbox-link" href="https://s.w.org/images/core/emoji/17.0.2/svg/1f9e1.svg" rel="noopener" tabindex="0" target="_blank"><img alt="&#x1f9e1;" class="emoji lazyloaded" draggable="false" src="https://s.w.org/images/core/emoji/17.0.2/svg/1f9e1.svg" /></a></p>
</div>
</div>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/sharepoint-framework-spfx-roadmap-update-april-2026/">SharePoint Framework (SPFx) roadmap update – April 2026</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
