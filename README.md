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

<h2>4.4.0&nbsp;Release Notes&nbsp;</h2>

<p><strong><strong>Release: </strong></strong>September, 2020</p>

<h3>General&nbsp;</h3>

<p>Version 4.4.0&nbsp;of the Pure Storage vSphere HTML Client Plugin supports vSphere (vCenter and ESXi) version 6.5 and later and Purity version 4.10&nbsp;and later.<br />
Users can upgrade to this version of the plugin from previous release version 4.x or higher. This version is certified by VMware.</p>

<h3>What’s New&nbsp;</h3>

<ul>
    <li>Support for ActiveDR&nbsp;
    <ul>
        <li>Provisioning datastores or copies</li>
        <li>Backend insights of datastore (show lag time, direction etc)</li>
        <li>Tolerance of volumes being in an ActiveDR&nbsp;pair</li>
    </ul>
    </li>
    <li>Create snapshot of a single vVol&nbsp;VMDK</li>
    <li>Set the ESXi host personality when creating new hosts in a new host group.</li>
</ul>

<h3>Fixed issues&nbsp;</h3>

<ul>
    <li><strong>Wrong status on verifying protocol-endpoint in creating vVol datastore. </strong>PE should show as not found when it has not been created yet.</li>
    <li><strong>Unable to Filter by VM Name in vSphere plugin. </strong>Filtering did not work when the VM was in a sub-folder.</li>
    <li><strong>Problems retrieving pods from other flasharrays in create datastore wizard if one array is offline or has api-token issue.</strong> If one array connection had an issue, the plugin would not find any pods on any healthy array.</li>
    <li><strong>Error loading array list. Seemingly arbitrary error when trying to perform plugin operations in linked mode. </strong>The underlying issue was that different vCenters would not coordinate responses and sometimes queries went to the wrong vCenter. The plugin now checks for the correct vCenter connection.</li>
    <li><strong>Create vVol snapshot button was missing. </strong>This was remove somewhat on purpose due to an old issue, that issue has been fully resolved and this feature has been returned.</li>
    <li><strong>Datastore&nbsp;type not disabled when user selects copy from VMFS snapshot. </strong>This allows the choice of vVols for a VMFS copy which is invalid, it no longer shows this option.</li>
    <li><strong>Error when resizing a datastore: Invalid Size, Size Must be a multiple of 512. </strong>This was a regression and has been fixed.</li>
    <li><strong>Snapshot info missing when creating VMFS datastore from snapshot. </strong>Old plugin showed the snapshot information during the wizard, this has been added back.</li>
    <li><strong>Deletion of datastore requires manual rescan when host in maintenance mode. </strong>Maintenance mode hosts were skipped when removing datastores, they are now cleaned up.</li>
    <li><strong>Unable to create datastore in maintenance mode.</strong> If the chosen host was in maintenance mode, the creation would fail. This is now supported.</li>
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
