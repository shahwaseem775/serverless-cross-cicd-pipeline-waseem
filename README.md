<!-- Instructions to deploy this project to multi account using cross account pipelines -->
1: create a code commit repo in tools account and add the project file .

2: deploy ./cloudformation/cf-CrossAccountRole/yml to target account .. it will require tools account Id and will create cross account role which will have tools account in its trust relationship

3: deploy ./cloudformation/template.yml to tools account after changing the parameters accordingly .. like target account id, codecommit url and Repository name etc . This template will create all the resourses like 2 different codebuild projects and codepipeline and s3 bucket.




