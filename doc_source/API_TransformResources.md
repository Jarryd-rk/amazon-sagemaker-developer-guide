# TransformResources<a name="API_TransformResources"></a>

Describes the resources, including ML instance types and ML instance count, to use for transform job\.

## Contents<a name="API_TransformResources_Contents"></a>

 **InstanceCount**   <a name="SageMaker-Type-TransformResources-InstanceCount"></a>
The number of ML compute instances to use in the transform job\. For distributed transform jobs, specify a value greater than 1\. The default value is `1`\.  
Type: Integer  
Valid Range: Minimum value of 1\.  
Required: Yes

 **InstanceType**   <a name="SageMaker-Type-TransformResources-InstanceType"></a>
The ML compute instance type for the transform job\. If you are using built\-in algorithms to transform moderately sized datasets, we recommend using ml\.m4\.xlarge or `ml.m5.large` instance types\.  
Type: String  
Valid Values:` ml.m4.xlarge | ml.m4.2xlarge | ml.m4.4xlarge | ml.m4.10xlarge | ml.m4.16xlarge | ml.c4.xlarge | ml.c4.2xlarge | ml.c4.4xlarge | ml.c4.8xlarge | ml.p2.xlarge | ml.p2.8xlarge | ml.p2.16xlarge | ml.p3.2xlarge | ml.p3.8xlarge | ml.p3.16xlarge | ml.c5.xlarge | ml.c5.2xlarge | ml.c5.4xlarge | ml.c5.9xlarge | ml.c5.18xlarge | ml.m5.large | ml.m5.xlarge | ml.m5.2xlarge | ml.m5.4xlarge | ml.m5.12xlarge | ml.m5.24xlarge`   
Required: Yes

 **VolumeKmsKeyId**   <a name="SageMaker-Type-TransformResources-VolumeKmsKeyId"></a>
The AWS Key Management Service \(AWS KMS\) key that Amazon SageMaker uses to encrypt data on the storage volume attached to the ML compute instance\(s\) that run the batch transform job\. The `VolumeKmsKeyId` can be any of the following formats:  
+ // KMS Key ID

   `"1234abcd-12ab-34cd-56ef-1234567890ab"` 
+ // Amazon Resource Name \(ARN\) of a KMS Key

   `"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab"` 
Type: String  
Length Constraints: Maximum length of 2048\.  
Pattern: `.*`   
Required: No

## See Also<a name="API_TransformResources_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/sagemaker-2017-07-24/TransformResources) 
+  [AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/sagemaker-2017-07-24/TransformResources) 
+  [AWS SDK for Go \- Pilot](https://docs.aws.amazon.com/goto/SdkForGoPilot/sagemaker-2017-07-24/TransformResources) 
+  [AWS SDK for Java](https://docs.aws.amazon.com/goto/SdkForJava/sagemaker-2017-07-24/TransformResources) 
+  [AWS SDK for Ruby V2](https://docs.aws.amazon.com/goto/SdkForRubyV2/sagemaker-2017-07-24/TransformResources) 