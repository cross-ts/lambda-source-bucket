# serverless-source-bucket
サーバレス関係のソースを管理するためのS3バケットを作るやつ  
e.g.) Lambdaのコード, cloudformation packageで作成するtemplate.yml

## Initialize
```
$ aws cloudformation create-stack \
  --stack-name <Your Stack Name> \
  --template-body file://cloudformation/s3.yml \
  --parameters \
    ParameterKey=BucketName,ParameterValue=<Your S3 Bucket Name>
```

## Delete
```
$ aws cloudformation delete-stack \
  --stack-name <Your Stack Name>
```
