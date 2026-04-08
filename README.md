# SAP Cloud Identity Services - IPS Jobs for SAP Concur
<!-- Please include descriptive title -->

[![REUSE status](https://api.reuse.software/badge/github.com/sap-samples/concur-joule-ips-jobs)](https://api.reuse.software/info/github.com/sap-samples/concur-joule-ips-jobs)


## Description
<!-- Please include SEO-friendly description -->
These are pre-configured provisioning jobs that you can import into Identity Provisioning. They require minimal configuration, based on your specific needs.
The jobs will first source users from Concur and create them in the local identity directory of your Cloud Identity instance. They will then provision the SAP Global ID back to the corresponding user in Concur. The Global ID is a prerequisite for using Joule and Task Center.

More detailed information for using the jobs can be found in the corresponding directories.

## Requirements
You will need 
1) An SAP Cloud Identity Services tenant and corresponding admin user.
2) An SAP Concur tenant and and corresponding admin user.



## Known Issues
<!-- You may simply state "No known issues. -->
No known issues

## How to obtain support
For complete documentation on these provisioning jobs, refer to the SAP Help portal:
1) [SAP Concur Source System](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/sap-concur?locale=en-US&version=LATEST)
2) [Local Identity Directory Source System](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/local-identity-directory?locale=en-US&version=LATEST)
3) [Local Identity Directory Target System](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/target-local-identity-directory?locale=en-US&version=LATEST)
4) [SAP Concur Target System](https://help.sap.com/docs/cloud-identity-services/cloud-identity-services/target-sap-concur?locale=en-US&version=LATEST)

If you need additional support with provisioning jobs, create a case with SAP Support using the component "BC-IAM-IPS". See [note 1296527](https://me.sap.com/notes/1296527/E) for additional details about how to create a support case.

## Contributing
This repository is provided "as-is".

## License
Copyright (c) 2026 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSE) file.
