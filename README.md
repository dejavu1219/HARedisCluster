#### Overview

1. [Redis](https://github.com/antirez/redis.git) 
2. [Sentinel](https://github.com/antirez/redis/blob/unstable/src/sentinel.c) is a tool supplied in redis source code, used for monitoring and failover automatically
3. [Twemproxy](https://github.com/twitter/twemproxy) is used as a proxy for redis
4. [Beholder](https://github.com/Serekh/beholder) can monitoring the output of Sentinel and restarting twemproxy to keep a persistent service

#### When you try to deploy ,just need to change the IP address in below files:

  hosts
  group_vars/redis_all


#### After that, please deploy like below:

  $ ansible-playbook redis.yml -i hosts --private-key=`your private key file`
