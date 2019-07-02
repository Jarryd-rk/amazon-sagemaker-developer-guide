# OutputDataConfig<a name="API_OutputDataConfig"></a>

Provides information about how to store model training results \(model artifacts\)\.

## Contents<a name="API_OutputDataConfig_Contents"></a>

 **KmsKeyId**   <a name="SageMaker-Type-OutputDataConfig-KmsKeyId"></a>
The AWS Key Management Service \(AWS KMS\) key that Amazon SageMaker uses to encrypt the model artifacts at rest using Amazon S3 server\-side encryption\. The `KmsKeyId` can be any of the following formats:   
+ // KMS Key ID

   `"1234abcd-12ab-34cd-56ef-1234567890ab"` 
+ // Amazon Resource Name \(ARN\) of a KMS Key

   `"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab"` 
+ // KMS Key Alias

   `"alias/ExampleAlias"` 
+ // Amazon Resource Name \(ARN\) of a KMS Key Alias

   `"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias"` 
If you use a KMS key ID or an alias of your master key, the Amazon SageMaker execution role must include permissions to call `kms:Encrypt`\. If you don't provide a KMS key ID, Amazon SageMaker uses the default KMS key for Amazon S3 for your role's account\. Amazon SageMaker uses server\-side encryption with KMS\-managed keys for `OutputDataConfig`\. If you use a bucket policy with an `s3:PutObject` permission that only allows objects with server\-side encryption, set the condition key of `s3:x-amz-server-side-encryption` to `"aws:kms"`\. For more information, see [KMS\-Managed Encryption Keys](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html) in the *Amazon Simple Storage Service Developer Guide\.*   
The KMS key policy must grant permission to the IAM role that you specify in your `CreateTrainingJob`, `CreateTransformJob`, or `CreateHyperParameterTuningJob` requests\. For more information, see [Using Key Policies in AWS KMS](http://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html) in the *AWS Key Management Service Developer Guide*\.  
Type: String  
Length Constraints: Maximum length of 2048\.  
Pattern: `.*`   
Required: No

 **S3OutputPath**   <a name="SageMaker-Type-OutputDataConfig-S3OutputPath"></a>
Identifies the S3 path where you want Amazon SageMaker to store the model artifacts\. For example, `s3://bucket-name/key-name-prefix`\.   
Type: String  
Length Constraints: Maximum length of 1024\.  
Pattern: `^(https|s3)://([^/]+)/?(.*)$`   
Required: Yes

## See Also<a name="API_OutputDataConfig_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/sagemaker-2017-07-24/OutputDataConfig) 
+  [AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/sagemaker-2017-07-24/OutputDataConfig) 
+  [AWS SDK for Go \- Pilot](https://docs.aws.amazon.com/goto/SdkForGoPilot/sagemaker-2017-07-24/OutputDataConfig) 
+  [AWS SDK for Java](https://docs.aws.amazon.com/goto/SdkForJava/sagemaker-2017-07-24/OutputDataConfig) 
+  [AWS SDK for Ruby V2](https://docs.aws.amazon.com/goto/SdkForRubyV2/sagemaker-2017-07-24/OutputDataConfig) 