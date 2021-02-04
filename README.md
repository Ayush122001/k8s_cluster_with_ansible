---------------------------------------------------------------------------------------------------------------------------------

# Ansible script for automating k8s cluster configuration over AWS                                                               
It will *povision OS* over AWS & *configure* one of them as *master* and other as *slave*
The only thing user need to do is to `create token` at master node & give it to slave node so that they can connect
 
 --------------------------------------------------------------------------------------------------------------------------------
 
 Things to do before running the script: 
 + change inventory path in ansible conf file to inv folder in this script
 + change(remote user) to ec2-user in ansible conf file
 + permission of key 400 & mention its path in ansible conf file
 + Run following cmd & give your `access_key` for dynamic inventory `export AWS_ACCESS_KEY_ID=""`
 + Run following cmd & give your `secret_key` for dynamic inventory `export export AWS_SECRET_ACCESS_KEY==""` 
 + Run following cmd & give your `region` for dynamic inventory `export export AWS_REGION""` 
 + And also provide info about access_key, secret_key, region, security group(sg), zone and key in variable file i.e. var.yml
 
---------------------------------------------------------------------------------------------------------------------------------
 
 ### If you want to increase your no. of slave then copy the code of slave as many no. of time as you want
 #### note: For now this script has capability to work on centos(7,8),rhel(7,8) & fedora  
 
 
 
