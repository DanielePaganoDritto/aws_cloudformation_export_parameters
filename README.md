# cloudformation_export_parameters
Cloudformation Template used to define and exports basic parameters to be reused for naming convention puproses. It allows to set and exports the following parameters:

- Project Name
- Environment (e.g. Development/Production)

it also creates an IAM Role to be used as a basic EC2 Role when creating instances. 

- RoleName: [Environment]_[Project]_EC2
- Default Role Policy: Ec2ReadOnlyAccess

Finally it show the following Outputs:

- RoleARN
- Project
- Environment
