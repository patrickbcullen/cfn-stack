# cfn-stack
Command line helper for CloudFormation that uses the AWS CLI and simplifies the creation and deletion of stacks.

## Install
```
wget https://github.com/patrickbcullen/cfn-stack/blob/master/cfn-stack
chmod +x cfn-stack
```

## Usage
```
cd myapp/
cfn-stack init
# edit cfn-stack.ini to fit your environment
cfn-stack up
cfn-stack down
```

## cfn-stack.ini
Cfn-stack uses a config file in the current directory called `cfn-stack.ini` to configure all the parameters for CloudFormation. You can create an initial version of this file with the `cfn-stack init` command or you can create it manually.

```
stack_name="my-stack"
region="us-east-1"
stack_template="my-template.yml"
template_config="my-config.yml"
```
