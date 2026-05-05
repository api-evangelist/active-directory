---
title: "Sponsor group type requirements for agent identities"
url: "https://devblogs.microsoft.com/microsoft365dev/sponsor-group-type-requirements-for-agent-identities/"
date: "Fri, 01 May 2026 17:45:01 +0000"
author: "Microsoft Entra Agent ID team"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p><span>As part of moving to general availability (GA) for Entra Agent ID, agent blueprints, agent blueprint principals, and agent identities only accept </span><b><span>dynamic membership groups</span></b><span> and </span><b><span>Microsoft 365 groups</span></b><span> as group-type sponsors. In addition, <strong>r</strong></span><b><span>ole-assignable groups </span></b><span>were supported during the Agent ID public preview but aren&#8217;t included in the GA release. </span><span> </span></p>
<h2><b><span>Why we&#8217;re making this change</span></b><span> </span></h2>
<p><span>Sponsors are a critical attribution mechanism in Agent ID. When an admin or automation queries &#8220;who is responsible for this agent?&#8221; or &#8220;which agents is this user responsible for?&#8221;, the sponsor relationship must resolve quickly and reliably to ensure a good experience. </span><span> </span></p>
<p><span>We&#8217;re making these changes to ensure the best performance while still enabling customers to use groups as sponsors of their Agent ID objects. Dynamic membership groups and Microsoft 365 groups are optimized for the patterns that sponsors require. By narrowing the supported set, we ensure that these operations remain fast and predictable as Agent ID adoption grows.</span><span> </span></p>
<h2><b><span>What this means for you</span></b><span> </span></h2>
<ul>
<li><b><span>New sponsor assignments</span></b><span> must use dynamic membership groups or Microsoft 365 groups. Attempts to assign other group types as sponsors will be rejected.</span><span> </span></li>
<li><b><span>Existing sponsors</span></b><span> from other group types that are already set on your agent identities or blueprints continue to function. No customer action is required.</span><span> </span></li>
<li><b><span>Individual users</span></b><span> remain fully supported as sponsors, with no changes.</span><span> </span></li>
</ul>
<h2><b><span>Recommended action and next steps</span></b><span> </span></h2>
<p><span>If your current workflows assign fixed-membership security groups or role-assignable groups as sponsors, transition to dynamic membership groups or Microsoft 365 groups before your next provisioning cycle. For details about how to configure sponsors, see </span><a href="https://learn.microsoft.com/en-us/entra/agent-id/agent-owners-sponsors-managers"><span style="font-size: 12pt;">Administrative relationships in Entra Agent ID</span></a><span>.</span><span> </span></p>
<p><span>We continue to accelerate the pace of development in Agent ID and Entra ID, and we plan to add support for new group types as Agent ID sponsors later this year. We also listen to customer feedback and will evaluate the priority of supporting role-assignable groups in the future. Watch this blog for updates!</span><span> </span></p>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/sponsor-group-type-requirements-for-agent-identities/">Sponsor group type requirements for agent identities</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
