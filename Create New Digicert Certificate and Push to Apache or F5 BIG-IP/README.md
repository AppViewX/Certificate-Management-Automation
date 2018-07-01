<h1><strong class="final-path">Create New Digicert Certificate and Push to Apache or F5 BIG-IP</strong></h1>
<h2>Description</h2>
<p>The DigiCert Certificate Creation workflow is used to enroll the DigiCert Certificate Authority (CA) with all the relevant Certificate Signing Request (CSR) details. On successful enrollment, the certificate will be retrieved from the CA and managed in the AppViewX Certificate inventory. Based on the user input the new certificate is pushed manually or automatically to the F5 or Apache server.<span class="Apple-converted-space">&nbsp;</span></p>
<h2><strong>Prerequisites</strong></h2>
<div>
<p>To run the DigiCert Certificate Creation workflow in your environment, ensure that the following prerequisites are met:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>Free AppViewX or AppViewX version 12.3.0 has been downloaded and installed.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The F5 BIG-IP device is added as managed entity in AppViewX ADC inventory</li>
<li>The DigiCert CA account has been configured in AppViewX</li>
<li>The Apache server is added as managed entity in AppViewX<span class="Apple-converted-space">&nbsp;Server inventory</span></li>
<li>An ITSM tool (ServiceNow) has been configured under the Change Management section of the AppViewX Settings module<span class="Apple-converted-space">&nbsp;</span></li>
<li>The DNS server you use must resolve the certificate domain name.<span class="Apple-converted-space">&nbsp;</span></li>
<li>Uncheck the &ldquo;Approval required&rdquo; parameter in the policy of the selected Certificate group to allow auto-implementation of the DigiCert Certificate Creation workflow.<span class="Apple-converted-space">&nbsp;</span></li>
<li>The standalone script push_file_to_apache.py must have been loaded in ~/aps/helper.<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
</div>
<h2><br /><strong>Compatible Software Versions</strong></h2>
<div>
<p>This workflow has been tested and validated on the following software versions:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>AppViewX &ndash; Free AppViewX and AVX 12.3.0<span class="Apple-converted-space">&nbsp;</span></li>
<li>F5 (both LTM and GTM) &ndash; version 11.x and 12.x<span class="Apple-converted-space">&nbsp;</span>&nbsp;</li>
<li>ServiceNow &ndash; Istanbul, Geneva, and Jakarta<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
<h2><strong>Limitations<span class="Apple-converted-space">&nbsp;</span></strong></h2>
<p>The DigiCert Certificate Creation workflow has the following limitations:<span class="Apple-converted-space">&nbsp;</span></p>
<ul>
<li>The duplicate certificates are not handled by an Application connector.<span class="Apple-converted-space">&nbsp;</span></li>
<li>User must approve F5 Apache Certificate Push and Apache Certificate Push provisioning template.<span class="Apple-converted-space">&nbsp;</span></li>
</ul>
</div>
