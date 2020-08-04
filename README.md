<!-- wp:heading -->
<h2></h2>
<!-- /wp:heading -->

<!-- wp:heading -->
<h2>Pure Storage FlashArray Plugin for the vSphere Client</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>The plugin is supported with the HTML-5 vSphere Client with versions vSphere 6.5 and later. For official support statements, please refer to the VMware compatibility guide here:</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><a href="https://www.vmware.com/resources/compatibility/search.php?deviceCategory=wcp&amp;details=1&amp;partners=399&amp;wcpfeatures=295&amp;page=1&amp;display_interval=10&amp;sortColumn=Partner&amp;sortOrder=Asc">https://www.vmware.com/resources/compatibility/search.php?deviceCategory=wcp&amp;details=1&amp;partners=399&amp;wcpfeatures=295&amp;page=1&amp;display_interval=10&amp;sortColumn=Partner&amp;sortOrder=Asc</a></p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:paragraph -->
<p>All FlashArray Purity versions that are currently in support by Pure Storage are supported by the plugin. Official support of vCenter versions follow VMware End of Life policies unless otherwise noted by Pure Storage.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Latest version 4.3.1 (May 21st, 2020)</strong></p>
<!-- /wp:paragraph -->
<h2>4.3.1&nbsp;Release Notes&nbsp;</h2>

<p><strong><strong>Release: </strong></strong>May, 2020</p>

<h3>General&nbsp;</h3>

<p>Version 4.3.1&nbsp;of the Pure Storage vSphere HTML Client Plugin supports vSphere (vCenter and ESXi) version 6.5 and later and Purity version 4.10&nbsp;and later.<br />
Users can upgrade to this version of the plugin from previous release version 4.x or higher. This version is certified by VMware.</p>

<h3>What’s New&nbsp;</h3>

<ul>
    <li>For the volume group manager, you can now filter by datastore name, not just volume or volume group name.</li>
    <li>First release also certified with vSphere&nbsp;6.5.</li>
</ul>

<h3>Fixed issues&nbsp;</h3>

<ul>
    <li>Errors in datastore provisioning wizard around loading FlashArray list, matching host groups, or creating the datastore, such as "<strong>String index out of range:"&nbsp;</strong>This was due to introduced code for NVMe-oF&nbsp;based datastores&nbsp;that caused lookups to fail if the type was unknown. This is fixed. Any customer experiencing generic "could not lookup object errors" should upgrade to this release. Multiple pathologies relate to this issue.</li>
    <li>The LUN ID was shown in the NVMe-oF datastore view, not the NVMe namespace&nbsp;ID. The namespace ID is now correctly shown.</li>
</ul>

<h3>Known issues&nbsp;</h3>

<ul>
    <li>Plugin does not offer custom per-feature permissions. Details <a href="/Solutions/VMware_Platform_Guide/User_Guides_for_VMware_Solutions/Using_the_Pure_Storage_Plugin_for_the_vSphere_Client/vSphere_Client:_Role-Based_Access_Control_(RBAC)" target="_blank" title="vSphere Client: Role-Based Access Control (RBAC)">here</a>.&nbsp;</li>
</ul>

<!-- /wp:list -->
<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->
<!-- wp:paragraph -->
<p><em>To report issues or request new features, please enter them here:</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><a href="https://github.com/PureStorage-Connect/vSphereClient-Plugin/issues">https://github.com/PureStorage-Connect/vSphereClient-Plugin/issues</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>For questions,&nbsp;<a href="https://codeinvite.purestorage.com/">join our Pure Storage Code Slack</a>&nbsp;team! Check out the #PowerCLI channel</p>
<!-- /wp:paragraph -->
