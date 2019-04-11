
# Description

Ansible playbooks to quickly deploy Citrix ADC services in Amazon Web Services (AWS)

> If you are looking for CloudFormation Templates to deploy Citrix ADC services in AWS, click [here](https://github.com/citrix/netscaler-aws-cloudformation)

## Pre-requisites

### Authentication

Please refer [here](https://docs.ansible.com/ansible/latest/scenario_guides/guide_aws.html#authentication) for the absible authentication documentation

### About the Playbooks

The playbooks are self-explanatory in nature. These below tips will help in understanding the playbooks faster

#### `state` parameter

By default, the state parameter is `present`. Meaning the resources are created
However, if the same resources are to be deleted, then pass the playbook with `state=absent`
Eg: `ansible-playbook <playbook-name.yaml> -e state=absent`

#### Input Parameter type

- `REQUIRED` - This parameter is mandatory
- `OPTIONAL` - This parameter is optional. The default status of this parameter will be in the respective comment section
- `CONDITIONAL` - This parameter is mandatory only for some conditions given in the comments, otherwise this is optional

### Custom Playbook

To edit/customize the playbook, please refer the documentation [here](https://docs.ansible.com/ansible/latest/modules/cloudformation_module.html)
