<h1>Easy Certificate Provisioning</h1>
<h2>Description</h2>
<p><br />The Easy Certificate Provisioning workflow creates a new certificate and binds it to multiple SSL profiles or Applications by passing simple inputs parameters like Common Name, device, SSL profile or application.&nbsp;</p>
<p>The workflow will accept the Common Name and create a new certificate using CA details specified in the certificate policy assigned to the requestor. It supports both internal and external Certificate Authorities. The assumption is only one cert group is assigned to the requestor and the CA settings are configured. Once the certificate is created, it is added to AppViewX inventory as managed cert. The workflow will either 'push' or 'push &amp; bind' this certificate to multiple devices of the same type (ADC / Server).&nbsp;</p>
<p><strong>Rollback - </strong>The rollback flow will remove the certificate&nbsp;from the pushed devices and revoke the&nbsp;certificate at CA.&nbsp;</p>
<h2>Prerequisites</h2>
<p><br />To run this automation workflow in your environment, ensure that the following pre-requisites are met:</p>
<ol>
<li>AppViewX version 12.4 has been downloaded and installed.</li>
<li>The F5 BIG-IP or Citrix ADC devices are added to the AppViewX inventory as managed entities.</li>
<li>Apache or TomCat servers are added in the inventory as managed entities.</li>
<li>The DigiCert, Ejbca, AppViewX or Comodo certificate manager accounts are configured on AppViewX</li>
<li>The&nbsp;appropriate user, user group, role, and resources are created and mapped correctly.</li>
<li>Certificate Group and Policy should be created and mapped with appropriate resources</li>
<li>For auto-implementation of this workflow &ldquo;Approval required&rdquo; parameter in the certificate policy must be unchecked&nbsp;</li>
<li>Certificate Policy should have correct values based on the CA selected for successful CSR generation and submission to the CA.</li>
<li>Update the helper &ldquo;easy_cert_helper&rdquo; with appropriate EJBCA detail and TomCat Detail.</li>
<li>You have administrator permissions to add a device to the AppViewX inventory.</li>
</ol>
<h2>Compatible Software Versions</h2>
<p>The workflow has been tested and validated on the following software versions:</p>
<ol>
<li>AppViewX &ndash;&nbsp; AVX 12.4</li>
<li>F5 &ndash; Version&nbsp; 11.x, 12.x or 13.X</li>
<li>Citrix &ndash; V11, V12&nbsp;</li>
</ol>
<h2>Limitations</h2>
<div>The workflow&nbsp;scope is limited to the following vendors&nbsp;</div>
<div>
<ul>
<li>CA -&nbsp;AppViewX,&nbsp;DigiCert,&nbsp;CCM,&nbsp;EJB<wbr />CA&nbsp;</li>
<li>ADCs - F5, Citrix&nbsp;</li>
<li>Servers -&nbsp;Apache, Tomcat&nbsp;</li>
</ul>
</div>
<h2>&nbsp;</h2>
