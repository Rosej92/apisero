# AWS S3 details:

AWS S3 Bucket:
1. bucket-rose2
2. bucket-rose-jacob

Topic
MuleTestTopic-147

ARN
arn:aws:sns:ap-south-1:211556697089:MuleTestTopic-147

Subscription: c4ec88f4-f99a-4acc-a3e4-f843ee4ab630

LOG:

14:01:39.519     11/17/2019     Worker-0     [MuleRuntime].io.03: [poc-aws-suite-api].create-object-demoFlow.BLOCKING @6deefd10     WARN
event:ad078ad0-0914-11ea-903e-0ab76ac35a9c No content length specified for stream data.  Stream contents will be buffered in memory and could result in out of memory errors.
14:01:40.279     11/17/2019     Worker-0     [MuleRuntime].io.03: [poc-aws-suite-api].create-object-demoFlow.BLOCKING @6deefd10     ERROR
event:ad078ad0-0914-11ea-903e-0ab76ac35a9c 
********************************************************************************
Message               : The component 'createObject' from the connector 'Amazon S3' attempted to throw 'S3:ANY', but it was not registered in the Error Repository.
Element               : create-object-demoFlow/processors/0 @ poc-aws-suite-api:poc-aws-suite-api.xml:33 (Create object)
Element XML           : <s3:create-object doc:name="Create object" doc:id="66fc98a7-49ff-478c-a0a0-5124b04d9078" config-ref="Amazon_S3_Configuration" bucketName="bucket-rose2" key="JsonTestMessage"></s3:create-object>
Error type            : MULE:UNKNOWN
Payload Type          : org.mule.runtime.core.internal.streaming.bytes.ManagedCursorStreamProvider
--------------------------------------------------------------------------------
Root Exception stack trace:
com.amazonaws.services.s3.model.AmazonS3Exception: The authorization header is malformed; the region 'us-east-1' is wrong; expecting 'ap-northeast-2' (Service: Amazon S3; Status Code: 400; Error Code: AuthorizationHeaderMalformed; Request ID: AA8FFC30DC1D797F; S3 Extended Request ID: jyRMrA//Xz95O/nJ3TI0RopJBVnDte73afd6N83GXlb7e9WMcGqEYUHMyN2QR6qWBbGbVO+Bkyo=), S3 Extended Request ID: jyRMrA//Xz95O/nJ3TI0RopJBVnDte73afd6N83GXlb7e9WMcGqEYUHMyN2QR6qWBbGbVO+Bkyo=

