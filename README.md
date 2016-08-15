#Hello,

#Here are our given tasks.

#(1)	Create a Redis cluster with 1 master and 3 slaves *	The cluster should have the capability to promote slaves to master automatically in the event of master going down for whatever reason. 

#(2) Once complete please create a cloud formation template to launch the entire infrastructure and automate the whole process using chef recipes. 

#(3)	Upload code to github and add a README with clear instructions on how to setup etc. Once complete please send us the link.

#=> First of all we will create four EC2 Instances and from that 1 will be Master and 3 will be Slave servers.

#=> After that we will install Redis Cluster into them and than configure as a master and 3 slave servers by following steps from below link.

#https://www.digitalocean.com/community/tutorials/how-to-configure-a-redis-cluster-on-ubuntu-14-04

#=> Now we will create a CloudFormation template of whole Existing Infrastructure by using CloudFormer tool by following below link.

#http://www.tothenew.com/blog/using-aws-cloudformer-to-create-template-of-existing-infrastructure/

#=> Now at the end you will get CloudFormation Template saved in S3 bucket. 

#=> You have to change the permissions for the template by allocating policy " Anyone " to view/edit. So now anyone with that link can access that template. Here is the link.

# https://s3-us-west-2.amazonaws.com/testnclouds/cloudformer.template

#=> Now for automating whole process we will write Chef Recipe like below.
# 
