---
title: "Prepare your add-in for Outlook ribbon improvements"
url: "https://devblogs.microsoft.com/microsoft365dev/prepare-your-addin-for-outlook-ribbon-improvements/"
date: "Fri, 06 Mar 2026 21:43:22 +0000"
author: "Office Extensibility team"
feed_url: "https://devblogs.microsoft.com/microsoft365dev/feed/"
---
<p>We’re improving how add-ins appear on the ribbon in Outlook on the web and the new Outlook on Windows. These Outlook ribbon updates make add-ins easier to find and align the experience across Outlook clients. Improvements include:</p>
<ul>
<li>Showing the group name specified in your manifest for the add-in’s ribbon button (instead of the add-in name from Microsoft Marketplace).</li>
<li>Adding a dropdown next to the add-in button for quick access to the add-in’s commands.</li>
<li>Adding a similar dropdown in the overflow menu.</li>
</ul>
<p><a href="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/outlook-ribbon-improvements.webp"><img alt="outlook ribbon improvements image" class="size-full wp-image-25402 alignnone" height="120" src="https://devblogs.microsoft.com/microsoft365dev/wp-content/uploads/sites/73/2026/03/outlook-ribbon-improvements.webp" width="365" /></a></p>
<p>To make sure your add-in shows the intended group name when these updates take effect, review your manifest and update the group label if needed. Where the group name is specified depends on the type of manifest your add-in uses.</p>
<ul>
<li><strong><a href="https://learn.microsoft.com/office/dev/add-ins/develop/unified-manifest-overview">Unified manifest for Microsoft 365</a></strong>: The group name is specified in the <a href="https://learn.microsoft.com/microsoft-365/extensibility/schema/extension-ribbons-custom-tab-groups-item#label">label</a> property of the relevant group in <a href="https://learn.microsoft.com/microsoft-365/extensibility/schema/extension-ribbons-array-tabs-item#groups">extensions.ribbons.tabs.groups</a>. The following code is an example.</li>
</ul>
<pre class="prettyprint language-js" style="padding-left: 40px;"><code class="language-js">"extensions": [
  {
    …
    "ribbons": [
      {
        …
        "tabs": [
          {
            …
            "groups": [
              {
                "id": "msgComposeCmdGroup",
                "label": "Contoso Add-in",
                …
              }
            ]
          }
        ]
      }
    ]
  }
]
</code></pre>
<ul>
<li><a href="https://learn.microsoft.com/office/dev/add-ins/develop/xml-manifest-overview"><strong>Add-in only manifest</strong></a>: The group name is specified in the relevant group’s child <a href="https://learn.microsoft.com/javascript/api/manifest/group#label">&lt;Label&gt;</a> Its value is defined in the <a href="https://learn.microsoft.com/javascript/api/manifest/shortstrings">&lt;ShortStrings&gt;</a> section of <a href="https://learn.microsoft.com/javascript/api/manifest/resources">&lt;Resources&gt;</a>. The following code is an example.</li>
</ul>
<pre class="prettyprint language-js" style="padding-left: 40px;"><code class="language-js">&lt;ExtensionPoint xsi:type="MessageComposeCommandSurface"&gt;
    &lt;OfficeTab id="TabDefault"&gt;
        &lt;Group id="msgComposeCmdGroup"&gt;
            &lt;Label resid="GroupLabel"/&gt;
            …
        &lt;/Group&gt;
    &lt;/OfficeTab&gt;
&lt;/ExtensionPoint&gt;
…
&lt;Resources&gt;
  …
  &lt;bt:ShortStrings&gt;
    &lt;bt:String id="GroupLabel" DefaultValue="Contoso Add-in"/&gt;
  &lt;/bt:ShortStrings&gt;
&lt;/Resources&gt;
</code></pre>
<p>To learn more about these ribbon updates, watch the <a href="https://youtu.be/ER0ECLlMye0?si=0dOJ4d06CpqAPF97">February 2026 recording of the Office Add-ins community call</a>.</p>
<p>The post <a href="https://devblogs.microsoft.com/microsoft365dev/prepare-your-addin-for-outlook-ribbon-improvements/">Prepare your add-in for Outlook ribbon improvements</a> appeared first on <a href="https://devblogs.microsoft.com/microsoft365dev">Microsoft 365 Developer Blog</a>.</p>
