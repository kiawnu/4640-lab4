# 4640-lab4

# Ian Macdonald, Ernest Law, Kian Abdollahi 

## Setup 
Current AWS profile = acit4640_admin

## SSH Key command

1. Generate an ssh
``` ssh-keygen -t ed25519 -f ~/.ssh/<key-name> -C "<commnet-to-identify-key>" ```

2. Add the value in the public key file to line 9 of `cloud-config.yaml`

## Terraform commands

1. Initialize terraform
``` terraform init ```

2. Ensure the files are formatted to the standard style 
``` terraform fmt ```

3. Create a build plan 
``` terraform plan -out <plan-name> ```

4. Execute the plan
``` terraform apply <plan-name> ```

5. Connect to the instance using 
``` ssh -i ~/.ssh/<private-key> <user>@<host>```

6. Remove resources
``` terraform destroy```

