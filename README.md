<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_iam_policy.eks_cluster_describe_and_assume](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_policy) | resource |
| [aws_iam_role_policy_attachment.serviceAccountPolicyAttach](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_role_policy_attachment) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_cluster_arn"></a> [cluster\_arn](#input\_cluster\_arn) | arn to use for a given iam user, role, group or policy | `string` | n/a | yes |
| <a name="input_description"></a> [description](#input\_description) | Policy description | `string` | n/a | yes |
| <a name="input_local_policy_file_path"></a> [local\_policy\_file\_path](#input\_local\_policy\_file\_path) | The path of the local policy file in this module | `string` | `"policies/policy.json.tftpl"` | no |
| <a name="input_policy_name"></a> [policy\_name](#input\_policy\_name) | Name of the IAM Policy | `string` | n/a | yes |
| <a name="input_role_name"></a> [role\_name](#input\_role\_name) | Name of the Role to which a policy is attached | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_policy_arn"></a> [policy\_arn](#output\_policy\_arn) | n/a |
<!-- END_TF_DOCS -->