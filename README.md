# Community AWS Collection

The Ansible Community AWS collection includes a variety of Ansible content to help automate the management of AWS instances. This collection is maintained by the Ansible community.

AWS related modules and plugins supported by the Ansible Cloud team are in the [amazon.aws](https://github.com/ansible-collections/amazon.aws) collection.

<!--start requires_ansible-->
## Ansible version compatibility

This collection has been tested against following Ansible versions: **>=2.9.10**.

Plugins and modules within a collection may be tested with only specific Ansible versions.
A collection may contain metadata that identifies these versions.
PEP440 is the schema used to describe the versions of Ansible.
<!--end requires_ansible-->

## Python version compatibility

This collection depends on the AWS SDK for Python (Boto3 and Botocore).  Due to the
[AWS SDK Python Support Policy](https://aws.amazon.com/blogs/developer/python-support-policy-updates-for-aws-sdks-and-tools/)
this collection requires Python 3.6 or greater.

Amazon have also announced the end of support for
[Python less than 3.7](https://aws.amazon.com/blogs/developer/python-support-policy-updates-for-aws-sdks-and-tools/).
As such support for Python less than 3.7 by this collection has been deprecated and will be removed in a release
after 2023-05-31.

## AWS SDK version compatibility

Starting with the 2.0.0 releases of amazon.aws and community.aws, it is generally the collection's policy to support the versions of `botocore` and `boto3` that were released 12 months prior to the most recent major collection release, following semantic versioning (for example, 2.0.0, 3.0.0).

Version 5.0.0 of this collection supports `boto3 >= 1.18.0` and `botocore >= 1.21.0`

All support for the original AWS SDK `boto` was removed in release 4.0.0.

## Included content
<!--start collection content-->
### Connection plugins
Name | Description
--- | ---
[community.aws.aws_ssm](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.aws_ssm_connection.rst)|execute via AWS Systems Manager

### Modules
Name | Description
--- | ---
[community.aws.accessanalyzer_validate_policy_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.accessanalyzer_validate_policy_info_module.rst)|Performs validation of IAM policies
[community.aws.acm_certificate](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.acm_certificate_module.rst)|Upload and delete certificates in the AWS Certificate Manager service
[community.aws.acm_certificate_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.acm_certificate_info_module.rst)|Retrieve certificate information from AWS Certificate Manager service
[community.aws.api_gateway](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.api_gateway_module.rst)|Manage AWS API Gateway APIs
[community.aws.api_gateway_domain](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.api_gateway_domain_module.rst)|Manage AWS API Gateway custom domains
[community.aws.application_autoscaling_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.application_autoscaling_policy_module.rst)|Manage Application Auto Scaling Scaling Policies
[community.aws.autoscaling_complete_lifecycle_action](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_complete_lifecycle_action_module.rst)|Completes the lifecycle action of an instance
[community.aws.autoscaling_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_group_module.rst)|Create or delete AWS AutoScaling Groups (ASGs)
[community.aws.autoscaling_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_group_info_module.rst)|Gather information about EC2 Auto Scaling Groups (ASGs) in AWS
[community.aws.autoscaling_instance_refresh](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_instance_refresh_module.rst)|Start or cancel an EC2 Auto Scaling Group (ASG) instance refresh in AWS
[community.aws.autoscaling_instance_refresh_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_instance_refresh_info_module.rst)|Gather information about EC2 Auto Scaling Group (ASG) Instance Refreshes in AWS
[community.aws.autoscaling_launch_config](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_launch_config_module.rst)|Create or delete AWS Autoscaling Launch Configurations
[community.aws.autoscaling_launch_config_find](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_launch_config_find_module.rst)|Find AWS Autoscaling Launch Configurations
[community.aws.autoscaling_launch_config_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_launch_config_info_module.rst)|Gather information about AWS Autoscaling Launch Configurations
[community.aws.autoscaling_lifecycle_hook](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_lifecycle_hook_module.rst)|Create, delete or update AWS ASG Lifecycle Hooks
[community.aws.autoscaling_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_policy_module.rst)|Create or delete AWS scaling policies for Autoscaling groups
[community.aws.autoscaling_scheduled_action](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.autoscaling_scheduled_action_module.rst)|Create, modify and delete ASG scheduled scaling actions
[community.aws.aws_region_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.aws_region_info_module.rst)|Gather information about AWS regions
[community.aws.batch_compute_environment](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.batch_compute_environment_module.rst)|Manage AWS Batch Compute Environments
[community.aws.batch_job_definition](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.batch_job_definition_module.rst)|Manage AWS Batch Job Definitions
[community.aws.batch_job_queue](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.batch_job_queue_module.rst)|Manage AWS Batch Job Queues
[community.aws.cloudformation_exports_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudformation_exports_info_module.rst)|Read a value from CloudFormation Exports
[community.aws.cloudformation_stack_set](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudformation_stack_set_module.rst)|Manage groups of CloudFormation stacks
[community.aws.cloudfront_distribution](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudfront_distribution_module.rst)|Create, update and delete AWS CloudFront distributions
[community.aws.cloudfront_distribution_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudfront_distribution_info_module.rst)|Obtain facts about an AWS CloudFront distribution
[community.aws.cloudfront_invalidation](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudfront_invalidation_module.rst)|create invalidations for AWS CloudFront distributions
[community.aws.cloudfront_origin_access_identity](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudfront_origin_access_identity_module.rst)|Create, update and delete origin access identities for a CloudFront distribution
[community.aws.cloudfront_response_headers_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudfront_response_headers_policy_module.rst)|Create, update and delete response headers policies to be used in a Cloudfront distribution
[community.aws.cloudtrail](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudtrail_module.rst)|manage CloudTrail create, delete, update
[community.aws.cloudwatch_metric_alarm](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudwatch_metric_alarm_module.rst)|Create/update or delete AWS CloudWatch 'metric alarms'
[community.aws.cloudwatchevent_rule](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudwatchevent_rule_module.rst)|Manage CloudWatch Event rules and targets
[community.aws.cloudwatchlogs_log_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudwatchlogs_log_group_module.rst)|create or delete log_group in CloudWatchLogs
[community.aws.cloudwatchlogs_log_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudwatchlogs_log_group_info_module.rst)|Get information about log_group in CloudWatchLogs
[community.aws.cloudwatchlogs_log_group_metric_filter](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.cloudwatchlogs_log_group_metric_filter_module.rst)|Manage CloudWatch log group metric filter
[community.aws.codebuild_project](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.codebuild_project_module.rst)|Create or delete an AWS CodeBuild project
[community.aws.codecommit_repository](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.codecommit_repository_module.rst)|Manage repositories in AWS CodeCommit
[community.aws.codepipeline](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.codepipeline_module.rst)|Create or delete AWS CodePipelines
[community.aws.config_aggregation_authorization](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.config_aggregation_authorization_module.rst)|Manage cross-account AWS Config authorizations
[community.aws.config_aggregator](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.config_aggregator_module.rst)|Manage AWS Config aggregations across multiple accounts
[community.aws.config_delivery_channel](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.config_delivery_channel_module.rst)|Manage AWS Config delivery channels
[community.aws.config_recorder](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.config_recorder_module.rst)|Manage AWS Config Recorders
[community.aws.config_rule](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.config_rule_module.rst)|Manage AWS Config rule resources
[community.aws.data_pipeline](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.data_pipeline_module.rst)|Create and manage AWS Datapipelines
[community.aws.directconnect_confirm_connection](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.directconnect_confirm_connection_module.rst)|Confirms the creation of a hosted DirectConnect connection
[community.aws.directconnect_connection](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.directconnect_connection_module.rst)|Creates, deletes, modifies a DirectConnect connection
[community.aws.directconnect_gateway](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.directconnect_gateway_module.rst)|Manage AWS Direct Connect gateway
[community.aws.directconnect_link_aggregation_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.directconnect_link_aggregation_group_module.rst)|Manage Direct Connect LAG bundles
[community.aws.directconnect_virtual_interface](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.directconnect_virtual_interface_module.rst)|Manage Direct Connect virtual interfaces
[community.aws.dms_endpoint](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.dms_endpoint_module.rst)|Creates or destroys a data migration services endpoint
[community.aws.dms_replication_subnet_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.dms_replication_subnet_group_module.rst)|creates or destroys a data migration services subnet group
[community.aws.dynamodb_table](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.dynamodb_table_module.rst)|Create, update or delete AWS Dynamo DB tables
[community.aws.dynamodb_ttl](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.dynamodb_ttl_module.rst)|Set TTL for a given DynamoDB table
[community.aws.ec2_ami_copy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_ami_copy_module.rst)|copies AMI between AWS regions, return new image id
[community.aws.ec2_customer_gateway](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_customer_gateway_module.rst)|Manage an AWS customer gateway
[community.aws.ec2_customer_gateway_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_customer_gateway_info_module.rst)|Gather information about customer gateways in AWS
[community.aws.ec2_eip](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_eip_module.rst)|manages EC2 elastic IP (EIP) addresses.
[community.aws.ec2_eip_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_eip_info_module.rst)|List EC2 EIP details
[community.aws.ec2_launch_template](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_launch_template_module.rst)|Manage EC2 launch templates
[community.aws.ec2_placement_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_placement_group_module.rst)|Create or delete an EC2 Placement Group
[community.aws.ec2_placement_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_placement_group_info_module.rst)|List EC2 Placement Group(s) details
[community.aws.ec2_snapshot_copy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_snapshot_copy_module.rst)|Copies an EC2 snapshot and returns the new Snapshot ID
[community.aws.ec2_transit_gateway](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_transit_gateway_module.rst)|Create and delete AWS Transit Gateways
[community.aws.ec2_transit_gateway_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_transit_gateway_info_module.rst)|Gather information about ec2 transit gateways in AWS
[community.aws.ec2_transit_gateway_vpc_attachment](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_transit_gateway_vpc_attachment_module.rst)|Create and delete AWS Transit Gateway VPC attachments
[community.aws.ec2_transit_gateway_vpc_attachment_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_transit_gateway_vpc_attachment_info_module.rst)|describes AWS Transit Gateway VPC attachments
[community.aws.ec2_vpc_egress_igw](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_egress_igw_module.rst)|Manage an AWS VPC Egress Only Internet gateway
[community.aws.ec2_vpc_nacl](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_nacl_module.rst)|create and delete Network ACLs
[community.aws.ec2_vpc_nacl_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_nacl_info_module.rst)|Gather information about Network ACLs in an AWS VPC
[community.aws.ec2_vpc_peer](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_peer_module.rst)|create, delete, accept, and reject VPC peering connections between two VPCs.
[community.aws.ec2_vpc_peering_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_peering_info_module.rst)|Retrieves AWS VPC Peering details using AWS methods.
[community.aws.ec2_vpc_vgw](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_vgw_module.rst)|Create and delete AWS VPN Virtual Gateways
[community.aws.ec2_vpc_vgw_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_vgw_info_module.rst)|Gather information about virtual gateways in AWS
[community.aws.ec2_vpc_vpn](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_vpn_module.rst)|Create, modify, and delete EC2 VPN connections
[community.aws.ec2_vpc_vpn_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_vpc_vpn_info_module.rst)|Gather information about VPN Connections in AWS.
[community.aws.ec2_win_password](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ec2_win_password_module.rst)|Gets the default administrator password for EC2 Windows instances
[community.aws.ecs_attribute](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_attribute_module.rst)|manage ecs attributes
[community.aws.ecs_cluster](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_cluster_module.rst)|Create or terminate ECS clusters.
[community.aws.ecs_ecr](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_ecr_module.rst)|Manage Elastic Container Registry repositories
[community.aws.ecs_service](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_service_module.rst)|Create, terminate, start or stop a service in ECS
[community.aws.ecs_service_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_service_info_module.rst)|List or describe services in ECS
[community.aws.ecs_tag](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_tag_module.rst)|create and remove tags on Amazon ECS resources
[community.aws.ecs_task](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_task_module.rst)|Run, start or stop a task in ECS
[community.aws.ecs_taskdefinition](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_taskdefinition_module.rst)|register a task definition in ecs
[community.aws.ecs_taskdefinition_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ecs_taskdefinition_info_module.rst)|Describe a task definition in ECS
[community.aws.efs](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.efs_module.rst)|create and maintain EFS file systems
[community.aws.efs_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.efs_info_module.rst)|Get information about Amazon EFS file systems
[community.aws.efs_tag](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.efs_tag_module.rst)|create and remove tags on Amazon EFS resources
[community.aws.eks_cluster](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.eks_cluster_module.rst)|Manage Elastic Kubernetes Service (EKS) Clusters
[community.aws.eks_fargate_profile](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.eks_fargate_profile_module.rst)|Manage EKS Fargate Profile
[community.aws.elasticache](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticache_module.rst)|Manage cache clusters in Amazon ElastiCache
[community.aws.elasticache_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticache_info_module.rst)|Retrieve information for AWS ElastiCache clusters
[community.aws.elasticache_parameter_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticache_parameter_group_module.rst)|Manage cache parameter groups in Amazon ElastiCache.
[community.aws.elasticache_snapshot](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticache_snapshot_module.rst)|Manage cache snapshots in Amazon ElastiCache
[community.aws.elasticache_subnet_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticache_subnet_group_module.rst)|manage ElastiCache subnet groups
[community.aws.elasticbeanstalk_app](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elasticbeanstalk_app_module.rst)|Create, update, and delete an Elastic Beanstalk application
[community.aws.elb_application_lb](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_application_lb_module.rst)|Manage an Application Load Balancer
[community.aws.elb_application_lb_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_application_lb_info_module.rst)|Gather information about Application Load Balancers in AWS
[community.aws.elb_classic_lb_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_classic_lb_info_module.rst)|Gather information about EC2 Elastic Load Balancers in AWS
[community.aws.elb_instance](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_instance_module.rst)|De-registers or registers instances from EC2 ELBs
[community.aws.elb_network_lb](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_network_lb_module.rst)|Manage a Network Load Balancer
[community.aws.elb_target](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_target_module.rst)|Manage a target in a target group
[community.aws.elb_target_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_target_group_module.rst)|Manage a target group for an Application or Network load balancer
[community.aws.elb_target_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_target_group_info_module.rst)|Gather information about ELB target groups in AWS
[community.aws.elb_target_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.elb_target_info_module.rst)|Gathers which target groups a target is associated with.
[community.aws.glue_connection](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.glue_connection_module.rst)|Manage an AWS Glue connection
[community.aws.glue_crawler](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.glue_crawler_module.rst)|Manage an AWS Glue crawler
[community.aws.glue_job](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.glue_job_module.rst)|Manage an AWS Glue job
[community.aws.iam_access_key](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_access_key_module.rst)|Manage AWS IAM User access keys
[community.aws.iam_access_key_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_access_key_info_module.rst)|fetch information about AWS IAM User access keys
[community.aws.iam_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_group_module.rst)|Manage AWS IAM groups
[community.aws.iam_managed_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_managed_policy_module.rst)|Manage User Managed IAM policies
[community.aws.iam_mfa_device_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_mfa_device_info_module.rst)|List the MFA (Multi-Factor Authentication) devices registered for a user
[community.aws.iam_password_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_password_policy_module.rst)|Update an IAM Password Policy
[community.aws.iam_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_policy_module.rst)|Manage inline IAM policies for users, groups, and roles
[community.aws.iam_policy_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_policy_info_module.rst)|Retrieve inline IAM policies for users, groups, and roles
[community.aws.iam_role](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_role_module.rst)|Manage AWS IAM roles
[community.aws.iam_role_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_role_info_module.rst)|Gather information on IAM roles
[community.aws.iam_saml_federation](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_saml_federation_module.rst)|Maintain IAM SAML federation configuration.
[community.aws.iam_server_certificate](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_server_certificate_module.rst)|Manage IAM server certificates for use on ELBs and CloudFront
[community.aws.iam_server_certificate_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_server_certificate_info_module.rst)|Retrieve the information of a server certificate
[community.aws.iam_user](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_user_module.rst)|Manage AWS IAM users
[community.aws.iam_user_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.iam_user_info_module.rst)|Gather IAM user(s) facts in AWS
[community.aws.inspector_target](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.inspector_target_module.rst)|Create, Update and Delete Amazon Inspector Assessment Targets
[community.aws.kinesis_stream](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.kinesis_stream_module.rst)|Manage a Kinesis Stream.
[community.aws.kms_key](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.kms_key_module.rst)|Perform various KMS key management tasks
[community.aws.kms_key_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.kms_key_info_module.rst)|Gather information about AWS KMS keys
[community.aws.lambda](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_module.rst)|Manage AWS Lambda functions
[community.aws.lambda_alias](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_alias_module.rst)|Creates, updates or deletes AWS Lambda function aliases
[community.aws.lambda_event](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_event_module.rst)|Creates, updates or deletes AWS Lambda function event mappings
[community.aws.lambda_execute](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_execute_module.rst)|Execute an AWS Lambda function
[community.aws.lambda_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_info_module.rst)|Gathers AWS Lambda function details
[community.aws.lambda_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lambda_policy_module.rst)|Creates, updates or deletes AWS Lambda policy statements.
[community.aws.lightsail](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lightsail_module.rst)|Manage instances in AWS Lightsail
[community.aws.lightsail_static_ip](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.lightsail_static_ip_module.rst)|Manage static IP addresses in AWS Lightsail
[community.aws.msk_cluster](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.msk_cluster_module.rst)|Manage Amazon MSK clusters
[community.aws.msk_config](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.msk_config_module.rst)|Manage Amazon MSK cluster configurations
[community.aws.networkfirewall](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_module.rst)|manage AWS Network Firewall firewalls
[community.aws.networkfirewall_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_info_module.rst)|describe AWS Network Firewall firewalls
[community.aws.networkfirewall_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_policy_module.rst)|manage AWS Network Firewall policies
[community.aws.networkfirewall_policy_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_policy_info_module.rst)|describe AWS Network Firewall policies
[community.aws.networkfirewall_rule_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_rule_group_module.rst)|create, delete and modify AWS Network Firewall rule groups
[community.aws.networkfirewall_rule_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.networkfirewall_rule_group_info_module.rst)|describe AWS Network Firewall rule groups
[community.aws.opensearch](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.opensearch_module.rst)|Creates OpenSearch or ElasticSearch domain
[community.aws.opensearch_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.opensearch_info_module.rst)|obtain information about one or more OpenSearch or ElasticSearch domain
[community.aws.rds_cluster](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_cluster_module.rst)|rds_cluster module
[community.aws.rds_cluster_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_cluster_info_module.rst)|Obtain information about one or more RDS clusters
[community.aws.rds_cluster_snapshot](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_cluster_snapshot_module.rst)|Manage Amazon RDS snapshots of DB clusters
[community.aws.rds_instance](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_instance_module.rst)|Manage RDS instances
[community.aws.rds_instance_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_instance_info_module.rst)|obtain information about one or more RDS instances
[community.aws.rds_instance_snapshot](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_instance_snapshot_module.rst)|Manage Amazon RDS instance snapshots
[community.aws.rds_option_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_option_group_module.rst)|Manages the creation, modification, deletion of RDS option groups
[community.aws.rds_option_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_option_group_info_module.rst)|rds_option_group_info module
[community.aws.rds_param_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_param_group_module.rst)|manage RDS parameter groups
[community.aws.rds_snapshot_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_snapshot_info_module.rst)|obtain information about one or more RDS snapshots
[community.aws.rds_subnet_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.rds_subnet_group_module.rst)|manage RDS database subnet groups
[community.aws.redshift](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.redshift_module.rst)|create, delete, or modify an Amazon Redshift instance
[community.aws.redshift_cross_region_snapshots](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.redshift_cross_region_snapshots_module.rst)|Manage Redshift Cross Region Snapshots
[community.aws.redshift_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.redshift_info_module.rst)|Gather information about Redshift cluster(s)
[community.aws.redshift_subnet_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.redshift_subnet_group_module.rst)|manage Redshift cluster subnet groups
[community.aws.route53](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.route53_module.rst)|add or delete entries in Amazons Route 53 DNS service
[community.aws.route53_health_check](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.route53_health_check_module.rst)|Manage health-checks in Amazons Route53 DNS service
[community.aws.route53_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.route53_info_module.rst)|Retrieves route53 details using AWS methods
[community.aws.route53_zone](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.route53_zone_module.rst)|add or delete Route53 zones
[community.aws.s3_bucket_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_bucket_info_module.rst)|Lists S3 buckets in AWS
[community.aws.s3_bucket_notification](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_bucket_notification_module.rst)|Creates, updates or deletes S3 Bucket notifications targeting Lambda functions, SNS or SQS.
[community.aws.s3_cors](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_cors_module.rst)|Manage CORS for S3 buckets in AWS
[community.aws.s3_lifecycle](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_lifecycle_module.rst)|Manage S3 bucket lifecycle rules in AWS
[community.aws.s3_logging](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_logging_module.rst)|Manage logging facility of an s3 bucket in AWS
[community.aws.s3_metrics_configuration](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_metrics_configuration_module.rst)|Manage s3 bucket metrics configuration in AWS
[community.aws.s3_sync](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_sync_module.rst)|Efficiently upload multiple files to S3
[community.aws.s3_website](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.s3_website_module.rst)|Configure an s3 bucket as a website
[community.aws.secretsmanager_secret](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.secretsmanager_secret_module.rst)|Manage secrets stored in AWS Secrets Manager
[community.aws.ses_identity](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ses_identity_module.rst)|Manages SES email and domain identity
[community.aws.ses_identity_policy](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ses_identity_policy_module.rst)|Manages SES sending authorization policies
[community.aws.ses_rule_set](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ses_rule_set_module.rst)|Manages SES inbound receipt rule sets
[community.aws.sns](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sns_module.rst)|Send Amazon Simple Notification Service messages
[community.aws.sns_topic](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sns_topic_module.rst)|Manages AWS SNS topics and subscriptions
[community.aws.sns_topic_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sns_topic_info_module.rst)|sns_topic_info module
[community.aws.sqs_queue](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sqs_queue_module.rst)|Creates or deletes AWS SQS queues
[community.aws.ssm_parameter](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.ssm_parameter_module.rst)|Manage key-value pairs in AWS Systems Manager Parameter Store
[community.aws.stepfunctions_state_machine](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.stepfunctions_state_machine_module.rst)|Manage AWS Step Functions state machines
[community.aws.stepfunctions_state_machine_execution](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.stepfunctions_state_machine_execution_module.rst)|Start or stop execution of an AWS Step Functions state machine
[community.aws.storagegateway_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.storagegateway_info_module.rst)|Fetch AWS Storage Gateway information
[community.aws.sts_assume_role](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sts_assume_role_module.rst)|Assume a role using AWS Security Token Service and obtain temporary credentials
[community.aws.sts_session_token](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.sts_session_token_module.rst)|Obtain a session token from the AWS Security Token Service
[community.aws.waf_condition](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.waf_condition_module.rst)|Create and delete WAF Conditions
[community.aws.waf_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.waf_info_module.rst)|Retrieve information for WAF ACLs, Rules, Conditions and Filters
[community.aws.waf_rule](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.waf_rule_module.rst)|Create and delete WAF Rules
[community.aws.waf_web_acl](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.waf_web_acl_module.rst)|Create and delete WAF Web ACLs
[community.aws.wafv2_ip_set](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_ip_set_module.rst)|wafv2_ip_set
[community.aws.wafv2_ip_set_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_ip_set_info_module.rst)|Get information about wafv2 ip sets
[community.aws.wafv2_resources](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_resources_module.rst)|wafv2_web_acl
[community.aws.wafv2_resources_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_resources_info_module.rst)|wafv2_resources_info
[community.aws.wafv2_rule_group](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_rule_group_module.rst)|wafv2_web_acl
[community.aws.wafv2_rule_group_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_rule_group_info_module.rst)|wafv2_web_acl_info
[community.aws.wafv2_web_acl](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_web_acl_module.rst)|Create and delete WAF Web ACLs
[community.aws.wafv2_web_acl_info](https://github.com/ansible-collections/community.aws/blob/main/docs/community.aws.wafv2_web_acl_info_module.rst)|wafv2_web_acl

<!--end collection content-->

## Installing this collection

You can install the AWS collection with the Ansible Galaxy CLI:

    ansible-galaxy collection install community.aws

You can also include it in a `requirements.yml` file and install it with `ansible-galaxy collection install -r requirements.yml`, using the format:

```yaml
---
collections:
  - name: community.aws

```

A specific version of the collection can be installed by using the `version` keyword in the `requirements.yml` file:

```yaml
---
collections:
  - name: community.aws
    version: 3.1.1
```

The python module dependencies are not installed by `ansible-galaxy`.  They can
be manually installed using pip:

    pip install requirements.txt

or:

    pip install boto3 botocore

## Using this collection

You can either call modules by their Fully Qualified Collection Namespace (FQCN), such as `community.aws.ec2_instance`, or you can call modules by their short name if you list the `community.aws` collection in the playbook's `collections` keyword:

```yaml
---
  - name: Create a DB instance using the default AWS KMS encryption key
    community.aws.rds_instance:
      id: test-encrypted-db
      state: present
      engine: mariadb
      storage_encrypted: True
      db_instance_class: db.t2.medium
      username: "{{ username }}"
      password: "{{ password }}"
      allocated_storage: "{{ allocated_storage }}"

```


### See Also:

* [Amazon Web Services Guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_aws.html)
* [Ansible Using collections](https://docs.ansible.com/ansible/latest/user_guide/collections_using.html) for more details.

## Contributing to this collection

We welcome community contributions to this collection. If you find problems, please open an issue or create a PR against the [Community AWS collection repository](https://github.com/ansible-collections/community.aws).
See [Contributing to Ansible-maintained collections](https://docs.ansible.com/ansible/devel/community/contributing_maintained_collections.html#contributing-maintained-collections) for more details.

You can also join us on:

- Libera.Chat IRC - the ``#ansible-aws`` [irc.libera.chat](https://libera.chat/) channel

### More information about contributing

- [Ansible Community Guide](https://docs.ansible.com/ansible/latest/community/index.html) - Details on contributing to Ansible
- [Contributing to Collections](https://docs.ansible.com/ansible/devel/dev_guide/developing_collections.html#contributing-to-collections) - How to check out collection git repositories correctly
- [Guidelines for Ansible Amazon AWS module development](https://docs.ansible.com/ansible/latest/dev_guide/platforms/aws_guidelines.html)
- [Getting Started With AWS Ansible Module Development and Community Contribution](https://www.ansible.com/blog/getting-started-with-aws-ansible-module-development)

## Release notes
<!--Add a link to a changelog.rst file or an external docsite to cover this information. -->

## Roadmap

<!-- Optional. Include the roadmap for this collection, and the proposed release/versioning strategy so users can anticipate the upgrade/update cycle. -->

## More information

- [Ansible Collection overview](https://github.com/ansible-collections/overview)
- [Ansible User guide](https://docs.ansible.com/ansible/latest/user_guide/index.html)
- [Ansible Developer guide](https://docs.ansible.com/ansible/latest/dev_guide/index.html)
- [Ansible Collection Developer Guide](https://docs.ansible.com/ansible/devel/dev_guide/developing_collections.html)
- [Ansible Community code of conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html)

## Licensing

GNU General Public License v3.0 or later.

See [COPYING](https://www.gnu.org/licenses/gpl-3.0.txt) to see the full text.
