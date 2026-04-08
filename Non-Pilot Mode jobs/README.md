# SAP Cloud Identity Services - IPS Jobs for SAP Concur - Not using Joule Pilot User mode


## Description
These are pre-configured provisioning jobs that you can import into Identity Provisioning. They require minimal configuration, based on your specific needs. These are intended for use when Joule Pilot Mode does not need to be used - the transformations are simpler (the entire group section is removed) and there's less risk for making unwanted / unintended changes to profile data in Concur.

The files should be imported in numerical order. Note that there are PROD and TEST versions of the Concur Source and Concur Target jobs - use the PROD versions if you're working in your Concur production entity (entity ID starts with a "p") and use the TEST versions if you're working in your Concur production sandbox entity (test site - entity ID starts with a "t"). 

After importing both the Concur source and target jobs, there are two properties you will need to update:
1) concur.company.id
2) concur.authorization.code

The values needed for these fields can be obtained by logging into Concur with an admin user and navigating to Administation -> Company -> Authentication Admin and then clicking on Company Request Token. Enter 

> **5bea7d57-6bc5-45ba-b5cf-91f04940fbf2**

in the App ID field and click Submit, and take note of the resulting Company UUID and Company Request Token Values.
Enter the Company UUID value in the concur.company.id property, and enter the Company Request Token Value in the concur.authorization.code value.
 

## Requirements
You will need 
1) An SAP Cloud Identity Services tenant and corresponding admin user.
2) An SAP Concur tenant and and corresponding admin user.



## Known Issues
<!-- You may simply state "No known issues. -->
No known issues

## How to obtain support
For complete documentation on these provisioning jobs, refer to the SAP Help portal:
1) [SAP Concur Source System ↗](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/sap-concur?locale=en-US&version=LATEST)
2) [Local Identity Directory Source System ↗](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/local-identity-directory?locale=en-US&version=LATEST)
3) [Local Identity Directory Target System ↗](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/target-local-identity-directory?locale=en-US&version=LATEST)
4) [SAP Concur Target System ↗](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/target-sap-concur?locale=en-US&version=LATEST)

If you need additional support with provisioning jobs, create a case with SAP Support using the component "BC-IAM-IPS". See [note 1296527 ↗](https://me.sap.com/notes/1296527/E) for additional details about how to create a support case.

## Contributing
This repository is provided "as-is".

## License
Copyright (c) 2026 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](../LICENSE) file.
