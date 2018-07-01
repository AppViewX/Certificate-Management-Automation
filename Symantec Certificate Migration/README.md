<h1><strong class="final-path">Symantec Certificate Migration</strong></h1>
<h2>Description</h2>
<p>The Symantec Migration workflow will migrate the Symantec certificate to the other CAs such as DigiCert, Entrust, Trustwave, and Comodo certificate manager, which are currently managed in the AppViewX instance. You can migrate up to 10 Symantec certificates using a single request.<span class="Apple-converted-space">&nbsp;</span></p>
<h2><strong>Prerequisites</strong></h2>
<div>
<p>To run this workflow, ensure that the following pre-requisites are met:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>Free AppViewX or AppViewX version 12.3.0 has been downloaded and installed.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The Symantec certificate must be discovered and managed in the AppViewX.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The DigiCert, Entrust, Trustwave, and Comodo certificate manager accounts are configured on AppViewX.<span class="Apple-converted-space">&nbsp;</span></li>
<li>Each CA must have the appropriate credentials.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The SMTP is configured in AppViewX for sending emails.<span class="Apple-converted-space">&nbsp;</span></li>
<li>&ldquo;Approval required&rdquo; parameter in the policy of the selected Certificate group must be unchecked for the auto-implementation of this workflow.<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
</div>
<h2><br /><strong>Compatible Software Versions</strong></h2>
<div>
<p>This workflow has been validated for the following software versions:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>AppViewX &ndash; Free AppViewX and AVX 12.3.0<span class="Apple-converted-space">&nbsp;</span></li>
<li>CAs - DigiCert, Entrust, Trustwave, and Comodo certificate managers<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
<p>&nbsp;</p>
<h2><strong>Limitations<span class="Apple-converted-space">&nbsp;</span></strong></h2>
<p>The workflow has the following limitations:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>App connector will not handle duplicate certificate for the same CA and CA cert type.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The inputs to generate the CSR may differ for Symantec and the migrated CA.<span class="Apple-converted-space">&nbsp;</span></li>
<li>In a single request, up to 10 Symantec certificates can be migrated.<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
</div>
