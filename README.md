[#](#) AWS crud-lambda's built by github pipeline

Revived my github account to get hands-on experience with aws, github workflows and the rust-sdk the AWS provides (as developer preview).
- On pushing this repo a github workflow should trigger a build off AWS-infrastrure using terraform
- While the build is orchestrated by a volatile ubuntu-instance the terraform-state is not kept automatically
- We need a terraform-cloud account in order to keep the necessary state (so infra doesn't get recreated when already running).
- git-hub needs a TF-KEY in order to get access to the terraform cloud account.
- terraform needs AWS-credentials in order to create infrastructure in the target account (AWS_ACCESS_KEY_ID && AWS_SECRET_ACCESS_KEY).
- Changed AWS-credentials within TF from terraform- to environment- . . . 
- Added AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY to github. NOT SURE WHY THIS SHOULD BE NEEDED
- on the other hand it is great that this can be tried out for free.

