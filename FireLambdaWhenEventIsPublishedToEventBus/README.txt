Fire Lambda when event is published to Event Bus Using Serverless Framework

1.) Install serverless framework.
2.) download template using 'serverless create --template aws-python3 --name python-library-lambda' command.
3.) Create one custom EventBus.
4.) Copy it's arn id and paste it in the serverless.yml file.
5.) deploy it using 'serverless deploy'.
6.) Run your python scripts and then you can see the output in CloudWatch logs.