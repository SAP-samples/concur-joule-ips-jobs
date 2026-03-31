# SAP Cloud Identity Services - IPS Jobs for SAP Concur
<!-- Please include descriptive title -->

<!--- Register repository https://api.reuse.software/register, then add REUSE badge:
[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/concur-joule-ips-jobs)](https://github.com/SAP-samples/concur-joule-ips-jobs)
-->

## Description
<!-- Please include SEO-friendly description -->
These are pre-configured provisioning jobs that you can import into Identity Provisioning. They require minimal configuration, based on your specific needs.
The jobs will first source users from Concur and create them in the local identity directory of your Cloud Identity instance. They will then provision the SAP Global ID back to the corresponding user in Concur. The Global ID is a prerequisite for using Joule and Task Center.

The files should be imported in numerical order. Note that there are PROD and TEST versions of the Concur Source and Concur Target jobs - use the PROD versions if you're working in your Concur production entity (entity ID starts with a "p") and use the TEST versions if you're working in your Concur production sandbox entity (test site - entity ID starts with a "t"). 

After importing the Concur jobs, there are two properties you will need to update:
1) concur.company.id
2) concur.authorization.code

The values needed for these fields can be obtained by logging into Concur with an admin user and navigating to Administation -> Company -> Authentication Admin and then clicking on Company Request Token. Enter 5bea7d57-6bc5-45ba-b5cf-91f04940fbf2 in the App ID field and click Submit, and take note of the resulting Company UUID and Company Request Token Values.
Enter the Company UUID value in the concur.company.id property, and enter the Company Request Token Value in the concur.authorization.code value.

## Requirements
You will need 
1) An SAP Cloud Identity Services tenant and corresponding admin user.
2) An SAP Concur tenant and and corresponding admin user.



## Known Issues
<!-- You may simply state "No known issues. -->
No known issues

## How to obtain support
If you need additional support with provisioning jobs, create a case with SAP Support using the component "BC-IAM-IPS". See [note 1296527](https://me.sap.com/notes/1296527/E) for additional details about how to create a support case.

## Contributing
This repository is provided "as-is".

## License
Copyright (c) 2026 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSE) file.
