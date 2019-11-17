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
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.handleErrorResponse(AmazonHttpClient.java:1712)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.executeOneRequest(AmazonHttpClient.java:1367)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.executeHelper(AmazonHttpClient.java:1113)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.doExecute(AmazonHttpClient.java:770)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.executeWithTimer(AmazonHttpClient.java:744)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.execute(AmazonHttpClient.java:726)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutor.access$500(AmazonHttpClient.java:686)
	at com.amazonaws.http.AmazonHttpClient$RequestExecutionBuilderImpl.execute(AmazonHttpClient.java:668)
	at com.amazonaws.http.AmazonHttpClient.execute(AmazonHttpClient.java:532)
	at com.amazonaws.http.AmazonHttpClient.execute(AmazonHttpClient.java:512)
	at com.amazonaws.services.s3.AmazonS3Client.invoke(AmazonS3Client.java:4926)
	at com.amazonaws.services.s3.AmazonS3Client.invoke(AmazonS3Client.java:4872)
	at com.amazonaws.services.s3.AmazonS3Client.access$300(AmazonS3Client.java:390)
	at com.amazonaws.services.s3.AmazonS3Client$PutObjectStrategy.invokeServiceCall(AmazonS3Client.java:5806)
	at com.amazonaws.services.s3.AmazonS3Client.uploadObject(AmazonS3Client.java:1794)
	at com.amazonaws.services.s3.AmazonS3Client.putObject(AmazonS3Client.java:1754)
	at org.mule.extension.s3.internal.connection.S3Connection.putObject(S3Connection.java:97)
	at org.mule.extension.s3.internal.service.ObjectServiceImpl.createObject(ObjectServiceImpl.java:94)
	at org.mule.connectors.atlantic.commons.builder.execution.PentaParamExecutionBuilder.lambda$withParam$0(PentaParamExecutionBuilder.java:39)
	at org.mule.connectors.atlantic.commons.builder.execution.TetraParamExecutionBuilder.lambda$withParam$0(TetraParamExecutionBuilder.java:39)
	at org.mule.connectors.atlantic.commons.builder.execution.TriParamExecutionBuilder.lambda$withParam$0(TriParamExecutionBuilder.java:39)
	at org.mule.connectors.atlantic.commons.builder.execution.BiParamExecutionBuilder.lambda$withParam$0(BiParamExecutionBuilder.java:39)
	at org.mule.connectors.atlantic.commons.builder.execution.MonoParamExecutionBuilder.lambda$withParam$0(MonoParamExecutionBuilder.java:35)
	at org.mule.connectors.atlantic.commons.builder.config.executor.DefaultExecutor.execute(DefaultExecutor.java:14)
	at org.mule.connectors.atlantic.commons.builder.execution.NoParamExecutionBuilder.execute(NoParamExecutionBuilder.java:32)
	at org.mule.connectors.atlantic.commons.builder.execution.MonoParamExecutionBuilder.withParam(MonoParamExecutionBuilder.java:38)
