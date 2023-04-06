# 1. AWS ECR
	  Create Repository
	  Private Or Public
    <Repository Name> Create Repository
# 2.IAM
  Create Role
  EC2
  Permissions policies
  EC2InstanceProfileForImageBuilderECRContainerBuilds
  OR
  Permissions policies > AmazonElasticContainerRegistryPublicPowerUser
  Name <ROLE NAME>
  Create Role
# 3.AWS ECR (If Private)
	  Open Repository
	  Permission
	  Add Statement
	  Account ID
	  IAM entities
    Select	<ROLE NAME>
	  Action > Select: ecr:BatchGetImages ecr:GetDownloadUrlForLayer
	  Save
# 4.AWS ECR (If Public)
	    Simply Access Access Image With ECR Image Name
      NOTE: If you are accessing ECR private image in K8s manifest. You must add other user’s Account ID in the ECR Repository.
