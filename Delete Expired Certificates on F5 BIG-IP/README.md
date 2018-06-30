<h1>Delete Expired Certificates on F5 BIG-IP</h1>
<h2>Description</h2>
<p><br />The Delete Expired Certificates on F5 BIG-IP workflow is used to delete the expired certificates and its associated SSL profiles and keys from an F5 device.</p>
<p>The configuration to delete the expired certificate and key from an F5 device are reviewed and approved at AppViewX. After the approval is granted, the workflow will delete the expired certificate from an F5 device. If an expired certificate is associated to any SSL profile, it is deleted from the F5 device only after the certificate and the key of that particular profile are replaced with the default certificate and key.</p>
<h2>Prerequisites</h2>
<p><br />To run this automation workflow in your environment, ensure that the following pre-requisites are met:<br />1) Free AppViewX or AppViewX version 12.3.0 has been downloaded and installed.<br />2) The ADC devices have been added to the AppViewX inventory with the data center name.<br />3) Each ADC device is a managed entity in AppViewX.<br />4) You have administrator permissions to add a device to the AppViewX inventory.</p>
<h2>Compatible Software Versions</h2>
<p><br />The workflow has been tested and validated on the following software versions:<br />1) AppViewX &ndash; Free AppViewX and AVX 12.3.0<br />2) F5 (both LTM and DNS) &ndash; Version 10.x, 11.x, or 12.x</p>
