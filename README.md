# quickstart-deloitte-truevoice

## TrueVoice on the AWS Cloud

Deploying this Quick Start sets up a registration integration used to provide registration and proposed on-boarding information for validation by the TrueVoice customer engagement team. After successful registration and TrueVoice due diligence procedures are complete, an AWS Service Catalog product will be made available to users, which provides a multipurpose TrueVoice PoV integration layer ready for use with AWS Connect, Corporate Data Centre or AWS Management Console uploads to S3:

The Quick Start sets up the following:

![](https://raw.githubusercontent.com/TVdelit01/aws-quickstart/connect-integration-deloitte-truevoice/assets/TrueVoice-on-AWS-Cloud-Architecture.png)


•	A registration stack consisting of a Custom Resource Lambda function that will invoke the TrueVoice PoV registration API and return a registration ID as a CloudFormation output.

After successful registration, an AWS Service Catalog Product will be made available to the account from where the Quick Start was launched providing a template that sets up the following:

•	An S3 bucket intended for integration with customer dedicated resources in the TrueVoice AWS Account and used as a staging area for audio files sourced from on-premises telephony systems or Amazon Connect.

•	A Lambda function tasked with transferring files from the integration bucket in the customer account into the TrueVoice AWS Account.

•	The required lambda IAM Execution Role to carry out the transfer from the integration bucket into the customer dedicated resources in the TrueVoice AWS Account.

For architectural details, best practices, step-by-step instructions, and customization options, see the [deployment guide](http://to-be-updated).

To post feedback, submit feature ideas, or report bugs, use the Issues section of this GitHub repo.

If you'd like to submit code for this Quick Start, please review the [AWS Quick Start Contributor's Guide](https://aws-quickstart.github.io/).