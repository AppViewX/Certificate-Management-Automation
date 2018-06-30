The Delete Expired Certificates on F5 BIG-IP workflow is used to delete the expired certificates and its associated SSL profiles and keys from an F5 device. 

The configuration to delete the expired certificate and key from an F5 device are reviewed and approved at AppViewX. After the approval is granted, the workflow will delete the expired certificate from an F5 device. If an expired certificate is associated to any SSL profile, it is deleted from the F5 device only after the certificate and the key of that particular profile are replaced with the default certificate and key.

Prerequisites
To run this automation workflow in your environment, ensure that the following pre-requisites are met:
1) Free AppViewX or AppViewX version 12.3.0 has been downloaded and installed.
2) The ADC devices have been added to the AppViewX inventory with the data center name.
3) Each ADC device is a managed entity in AppViewX.
4) You have administrator permissions to add a device to the AppViewX inventory.

Compatible Software Versions
The workflow has been tested and validated on the following software versions:
1) AppViewX – Free AppViewX and AVX 12.3.0
2) F5 (both LTM and DNS) – Version 10.x, 11.x, or 12.x
