<h1>CA to CA Certificate Migration</h1>
<h2>Description</h2>
<p>The CA to CA Certificate Migration workflow will migrate the certificates from one of the source CAs such as DigiCert, Entrust, EJBCA, Symantec, Trustwave, and Comodo certificate manager to the other target CAs (other than selected source CA) such as DigiCert, Entrust, Trustwave, and Comodo certificate manager, which are currently managed in AppViewX. The workflow provides an option to update the CSR generation parameters such as different key length or hash algorithm. The migration report is emailed to the user who has submitted the request. You can migrate up to 10 certificates from the selected source CA using a single request.<span class="Apple-converted-space">&nbsp;</span></p>
<p><strong>Note: </strong>The platform is capable of migrating more than 10 certificates in a single request. This is a sample workflow to showcase the platform capabilities.<span class="Apple-converted-space">&nbsp;</span></p>
<h2><strong>Prerequisites</strong></h2>
<div>
<p>To run this workflow in your environment, the following prerequisites must be met:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>The selected source CA certificates must have been discovered and added as managed certificates in AppViewX inventory.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The CA accounts - DigiCert, Entrust, EJBCA, Trustwave, and Comodo certificate manager are configured on AppViewX.<span class="Apple-converted-space">&nbsp;</span></li>
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
<li>CAs &ndash; DigiCert, Entrust, EJBCA, Trustwave, and Comodo certificate manager accounts<span class="Apple-converted-space">&nbsp;</span></li>
<li>ServiceNow &ndash; Geneva, Eureka, Istanbul, and Jakarta<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
<h2><strong>Limitations<span class="Apple-converted-space">&nbsp;</span></strong></h2>
<p>The workflow has the following limitations:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>App connector will not handle duplicate certificate for the same CA and CA certificate type.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The inputs to generate the CSR may differ for the migrated source and target CAs.<span class="Apple-converted-space">&nbsp;</span></li>
<li>In a single request, up to ten Symantec certificates can be migrated.<span class="Apple-converted-space">&nbsp;</span></li>
<li>Even if one certificate is successfully enrolled, retrieved from CA, and managed in Appviewx certificate inventory, the request and ServiceNow ticket will be considered complete.<span class="Apple-converted-space">&nbsp;</span></li>
<li>Start Time and End Time of ITSM has nothing do with the workflow implementation time. Once the ITSM ticket is approved, CA to CA migration will start working.<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
</div>
