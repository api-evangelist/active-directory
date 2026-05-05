---
title: "SharePoint Framework (SPFx) roadmap update – March 2026"
url: "https://devblogs.microsoft.com/microsoft365dev/sharepoint-framework-spfx-roadmap-update-march-2026/"
date: "Wed, 25 Mar 2026 04:57:28 +0000"
author: "Vesa Juvonen"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p><strong>March 2026 continues the momentum for the <a href="https://aka.ms/spfx">SharePoint Framework</a> and the broader Microsoft 365 ecosystem</strong>, with a strong mix of platform progress, community energy, and clear signals about where SPFx is heading next. As we move deeper into the year, SPFx remains a critical foundation for modern extensibility across Microsoft 365 &#8211; supporting secure, scalable, and increasingly AI‑powered solutions built by customers, partners, and the global developer community.</p>
<div>
<p>A key milestone this month is the release of <a href="https://learn.microsoft.com/en-us/sharepoint/dev/spfx/release-1.23"><strong>SPFx 1.23 Preview</strong></a>, which gives developers an early look at what’s coming next. Alongside the preview, we have now <strong>confirmed the schedule for the next release</strong>, with <strong>SPFx 1.23 planned to reach general availability on April 15th</strong>. While this represents a slight delay from the originally planned timeline, the focus remains on delivering the right level of quality, stability, and predictability that enterprise customers and partners expect. Thank you for your patience and for the continued feedback that helps us get this right.</p>
<p>March was also defined by greatly attended <a href="https://aka.ms/sharepoint/hackathon"><strong>SharePoint 2026 Hackathon</strong></a>. The energy, creativity, and quality of submissions across the community were truly inspiring. From AI‑powered scenarios to real‑world business solutions, the hackathon once again demonstrated the strength of the Microsoft 365, Copilot, SharePoint and SPFx ecosystem. A huge <strong>thank you to everyone who participated, shared, built, reviewed, and supported</strong> &#8211; this is “sharing is caring” at its very best.</p>
<p>We also had the opportunity to reconnect with many of our <strong>Microsoft MVPs during the <a href="https://summit.microsoft.com/">MVP Summit</a></strong>, and the feedback we received was both energizing and validating. Conversations around the <strong>future direction of SPFx</strong>, especially in the context of AI, Copilot, and evolving developer workflows, reinforced our commitment to continue evolving SPFx as a first‑class extensibility platform in the age of AI. Expect more to share soon &#8211; there are <strong>exciting announcements ahead</strong>.</p>
<p>Looking ahead, the next opportunities to meet, learn, and collaborate in person are just around the corner. We’re excited to see the community again at the <a href="https://m365conf.com/"><strong>Microsoft 365 Community Conference</strong></a> and the <a href="https://collabsummit.eu/"><strong>European Collaboration Summit</strong></a>, both of which continue to be key moments for connection, learning, and shaping what’s next together.</p>
<p>As always, <strong>thank you for your continued engagement, honest feedback, and passion for building on SharePoint and SPFx</strong>. The platform continues to evolve because of this community &#8211; and March was another strong reminder of just how powerful that collaboration is <img alt="🙏" class="wp-smiley" src="https://s.w.org/images/core/emoji/17.0.2/72x72/1f64f.png" style="height: 1em;" /></p>
</div>
<div>
<h2>Release of SPFx version 1.23 preview</h2>
<div>
<p>We are excited to share a first public preview of the upcoming SharePoint Framework 1.23 with following new features. If you have the option, please test out things and provide us feedback on them.</p>
<ul>
<li>Grouping support for list view command sets</li>
<li>Preview of new SPFx CLI and open-sourced templates</li>
<li>Addressing npm audit issues</li>
</ul>
</div>
</div>
<p>See details on the 1.22 release on the release notes:</p>
<ul>
<li><a href="https://learn.microsoft.com/en-us/sharepoint/dev/spfx/release-1.23">SharePoint Framework 1.23 preview release notes</a></li>
</ul>
<p>We are looking into providing general availability of 1.23 in mid-April with following planned schedule:</p>
<ul>
<li>April 1st &#8211; Beta 1 &#8211; planned to include list and library panel override support</li>
<li>April 8th &#8211; Release Candidate</li>
<li>April 15th &#8211; General availability</li>
</ul>
<p>This is the currently planned schedule but it can be still change based on the potential findings before the general availability release.</p>
<h2 id="roadmap">Roadmap</h2>
<p>We are evolving towards a quarterly release cycle, providing more predictability on new feature introductions and updates. We will update the <a href="https://learn.microsoft.com/en-us/sharepoint/dev/spfx/roadmap" rel="noopener" target="_blank">public roadmap</a> with any schedule and feature updates as we move forward in this journey.</p>
<p>Here is the set of investments which we are planning to ship within the upcoming SPFx releases:</p>
<h3 id="version-1.23-–-february/march-2026"><strong>Version 1.23 &#8211; April 2026</strong></h3>
<p>This release focuses on open sourcing the templates and tooling to create SPFx solutions, enabling our ecosystem to optionally build their own templates. We also want to focus on providing additional value for optimizing developer experience and providing new extensibility options.</p>
<ul>
<li><strong>Command set improvements</strong> for lists and libraries – grouping and potentially other improvements.</li>
<li>A new open-sourced <strong>SPFx CLI</strong> for replacing the existing Yeoman generator as <strong>preview release</strong> &#8211; You will be able to introduce your company specific templates or adjustments on the scaffolded baseline for the SPFx solutions. We are decoupling the CLI itself from the SPFx release versions. This might be included in the 1.23 initial release as well.</li>
<li><b>Open-source </b><b>SPFx solution templates to GitHub</b> (when SPFx CLI is used)</li>
<li><b>New and edit panel override support</b> for lists and libraries</li>
<li>Other technical updates (eslint update)</li>
<li>Addressing any new npm audit vulnerability issues</li>
</ul>
<h3 id="version-1.23-–-february/march-2026"><strong>Version 1.23.1 &#8211; April 2026</strong></h3>
<p>This is planned release on end of the April to address any potential new npm audit vulnerabilities &#8211; scheduled to happen on last week of April.</p>
<ul>
<li>Addressing any new npm audit vulnerability issues</li>
</ul>
<h3 id="version-1.24-–-may/june-2026"><strong>Version 1.24 &#8211; June 2026</strong></h3>
<p>This version continues providing new extensibility options aligned with the future direction of SharePoint. We are also expecting to have other new features and capabilities as part of this release, which will be disclosed a bit later.</p>
<ul>
<li><strong>Navigation customizers</strong> – Options to override navigation nodes and/or experiences with SPFx components.</li>
<li><strong>React 18</strong> support for SPFx solutions</li>
<li>SPFx CLI general availability (GA)</li>
<li>Addressing any new npm audit vulnerability issues</li>
<li>Other features will be shared later.</li>
</ul>
<p><strong>We also continue further innovation in the AI space</strong> with a focus on both customer features and developer tooling. More on this in future roadmap updates during 2026.</p>
<p>We encourage you to continue <strong>providing feedback to support our product planning for the upcoming semesters</strong>. We already have an extensive list of ideas and enhancements in mind but are always interested in your input.</p>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/spfx-2026-march-roadmap.webp"><img alt="spfx 2026 march roadmap image" class="alignnone size-large wp-image-25467" height="577" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/spfx-2026-march-roadmap-1024x577.webp" width="1024" /></a></p>
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
<p>We are looking forward on having discussions with you all at the Microsoft 365 Community Conference and in European Collaboration Summit 2026. Hoping to see you all there.</p>
<p>Follow us also on <a href="https://www.linkedin.com/showcase/microsoft365dev/" rel="noopener" target="_blank">LinkedIn</a> or in <a href="https://x.com/microsoft365dev" rel="noopener" target="_blank">X</a> to stay up to date on Microsoft 365 Platform announcements.</p>
<p>Got feedback or input on this blog post &#8211; leave a comment and we will get back to you <img alt="&#x1f64b;&#x200d;&#x2642;" class="emoji" draggable="false" src="https://s.w.org/images/core/emoji/17.0.2/svg/1f64b-200d-2642-fe0f.svg" /></p>
<p>Happy coding! <strong>Sharing is Caring!</strong> <a class="lightbox-link" href="https://s.w.org/images/core/emoji/17.0.2/svg/1f9e1.svg" rel="noopener" tabindex="0" target="_blank"><img alt="&#x1f9e1;" class="emoji lazyloaded" draggable="false" src="https://s.w.org/images/core/emoji/17.0.2/svg/1f9e1.svg" /></a></p>
</div>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/sharepoint-framework-spfx-roadmap-update-march-2026/">SharePoint Framework (SPFx) roadmap update – March 2026</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
