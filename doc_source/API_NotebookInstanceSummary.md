# NotebookInstanceSummary<a name="API_NotebookInstanceSummary"></a>

Provides summary information for an Amazon SageMaker notebook instance\.

## Contents<a name="API_NotebookInstanceSummary_Contents"></a>

 **AdditionalCodeRepositories**   <a name="SageMaker-Type-NotebookInstanceSummary-AdditionalCodeRepositories"></a>
An array of up to three Git repositories associated with the notebook instance\. These can be either the names of Git repositories stored as resources in your account, or the URL of Git repositories in [AWS CodeCommit](http://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html) or in any other Git repository\. These repositories are cloned at the same level as the default repository of your notebook instance\. For more information, see [Associating Git Repositories with Amazon SageMaker Notebook Instances](http://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html)\.  
Type: Array of strings  
Array Members: Maximum number of 3 items\.  
Length Constraints: Minimum length of 1\. Maximum length of 1024\.  
Pattern: `^https://([^/]+)/?(.*)$|^[a-zA-Z0-9](-*[a-zA-Z0-9])*`   
Required: No

 **CreationTime**   <a name="SageMaker-Type-NotebookInstanceSummary-CreationTime"></a>
A timestamp that shows when the notebook instance was created\.  
Type: Timestamp  
Required: No

 **DefaultCodeRepository**   <a name="SageMaker-Type-NotebookInstanceSummary-DefaultCodeRepository"></a>
The Git repository associated with the notebook instance as its default code repository\. This can be either the name of a Git repository stored as a resource in your account, or the URL of a Git repository in [AWS CodeCommit](http://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html) or in any other Git repository\. When you open a notebook instance, it opens in the directory that contains this repository\. For more information, see [Associating Git Repositories with Amazon SageMaker Notebook Instances](http://docs.aws.amazon.com/sagemaker/latest/dg/nbi-git-repo.html)\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 1024\.  
Pattern: `^https://([^/]+)/?(.*)$|^[a-zA-Z0-9](-*[a-zA-Z0-9])*`   
Required: No

 **InstanceType**   <a name="SageMaker-Type-NotebookInstanceSummary-InstanceType"></a>
The type of ML compute instance that the notebook instance is running on\.  
Type: String  
Valid Values:` ml.t2.medium | ml.t2.large | ml.t2.xlarge | ml.t2.2xlarge | ml.t3.medium | ml.t3.large | ml.t3.xlarge | ml.t3.2xlarge | ml.m4.xlarge | ml.m4.2xlarge | ml.m4.4xlarge | ml.m4.10xlarge | ml.m4.16xlarge | ml.m5.xlarge | ml.m5.2xlarge | ml.m5.4xlarge | ml.m5.12xlarge | ml.m5.24xlarge | ml.c4.xlarge | ml.c4.2xlarge | ml.c4.4xlarge | ml.c4.8xlarge | ml.c5.xlarge | ml.c5.2xlarge | ml.c5.4xlarge | ml.c5.9xlarge | ml.c5.18xlarge | ml.c5d.xlarge | ml.c5d.2xlarge | ml.c5d.4xlarge | ml.c5d.9xlarge | ml.c5d.18xlarge | ml.p2.xlarge | ml.p2.8xlarge | ml.p2.16xlarge | ml.p3.2xlarge | ml.p3.8xlarge | ml.p3.16xlarge`   
Required: No

 **LastModifiedTime**   <a name="SageMaker-Type-NotebookInstanceSummary-LastModifiedTime"></a>
A timestamp that shows when the notebook instance was last modified\.  
Type: Timestamp  
Required: No

 **NotebookInstanceArn**   <a name="SageMaker-Type-NotebookInstanceSummary-NotebookInstanceArn"></a>
The Amazon Resource Name \(ARN\) of the notebook instance\.  
Type: String  
Length Constraints: Maximum length of 256\.  
Required: Yes

 **NotebookInstanceLifecycleConfigName**   <a name="SageMaker-Type-NotebookInstanceSummary-NotebookInstanceLifecycleConfigName"></a>
The name of a notebook instance lifecycle configuration associated with this notebook instance\.  
For information about notebook instance lifestyle configurations, see [Step 2\.1: \(Optional\) Customize a Notebook Instance](https://docs.aws.amazon.com/sagemaker/latest/dg/notebook-lifecycle-config.html)\.  
Type: String  
Length Constraints: Maximum length of 63\.  
Pattern: `^[a-zA-Z0-9](-*[a-zA-Z0-9])*`   
Required: No

 **NotebookInstanceName**   <a name="SageMaker-Type-NotebookInstanceSummary-NotebookInstanceName"></a>
The name of the notebook instance that you want a summary for\.  
Type: String  
Length Constraints: Maximum length of 63\.  
Pattern: `^[a-zA-Z0-9](-*[a-zA-Z0-9])*`   
Required: Yes

 **NotebookInstanceStatus**   <a name="SageMaker-Type-NotebookInstanceSummary-NotebookInstanceStatus"></a>
The status of the notebook instance\.  
Type: String  
Valid Values:` Pending | InService | Stopping | Stopped | Failed | Deleting | Updating`   
Required: No

 **Url**   <a name="SageMaker-Type-NotebookInstanceSummary-Url"></a>
The URL that you use to connect to the Jupyter instance running in your notebook instance\.   
Type: String  
Required: No

## See Also<a name="API_NotebookInstanceSummary_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/sagemaker-2017-07-24/NotebookInstanceSummary) 
+  [AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/sagemaker-2017-07-24/NotebookInstanceSummary) 
+  [AWS SDK for Go \- Pilot](https://docs.aws.amazon.com/goto/SdkForGoPilot/sagemaker-2017-07-24/NotebookInstanceSummary) 
+  [AWS SDK for Java](https://docs.aws.amazon.com/goto/SdkForJava/sagemaker-2017-07-24/NotebookInstanceSummary) 
+  [AWS SDK for Ruby V2](https://docs.aws.amazon.com/goto/SdkForRubyV2/sagemaker-2017-07-24/NotebookInstanceSummary) 