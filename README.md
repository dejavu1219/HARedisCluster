#### Overview

1. Redis 
2. Sentinel is a tool supplied in redis source code, used for monitoring and failover automatically
3. Twemproxy is used as a proxy for redis
4. Beholder can monitoring the output of Sentinel and restarting twemproxy to keep a persistent service

#### When you try to deploy ,just need to change the IP address in below files:

	hosts
	group_vars/redis_all


#### After that, please deploy like below:

	$ ansible-playbook redis.yml -i hosts --private-key=`your private key file`
