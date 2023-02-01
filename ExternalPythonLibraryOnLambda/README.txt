How to install External Python library such as Pandas on AWS lambda using serverless framework

1.) Install serverless framework.
2.) download template using 'serverless create --template aws-python3 --name python-library-lambda' command
3.) Update handler function by importing any module and Import unzip_requirements must be called as we are using zipped requirements.
4.) In serverless.yml under package->include, give moduled you have imported.
5.) In same file under custom->pythonRequirements, provide dockerizePip and zip as true.
6.) Install the serverless-python-requirements using 'serverless plugin install -n serverless-python-requirements' command and mention it under plugins.
7.) Create a requirements.txt and in that, mention the mudule you imported in a function along with its version.
8.) Deploy the function using "serverless deploy'
9.) Call it locally using 'serverless invoke local --function hello' command