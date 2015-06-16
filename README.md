#### When you try to deploy ,just need to change the IP address in below files:

	hosts
	group_vars/redis_all


#### After that, please deploy like below:

	$ ansible-playbook redis.yml -i hosts --private-key=`your private key file`
