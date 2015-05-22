# A Scalable and Resilient Microservice Environment with Apache Mesos and Apache Aurora

starts with background of existing infra

mesos used by lots of companies - apple, twitter, netflix

resources - cpu, memory, disk, ports

attributes - host, rack, os, disk type - attributes fixed to machine

twitter project to provide mysql cluster on mesos

https://github.com/twitter/mysos

http://aurora.apache.org/

auroroa scheduler for mesos

"Apache Aurora is a Mesos framework for long-running services and cron jobs."

discovery via zookeeper

does rolling updates / rollbacks, same as kubernetes

constraints are combination of attributes / resources

thrift api or rest

aurora seems to do crons

actually seems really cool - http://aurora.apache.org/documentation/latest/cron-jobs/

gives you a centralised dashboard of the crons that have run

they are doing 100 deploys a day, 10 minutes commit -> prod

they dont use docker - just run a single jar file

would like to run coreos on mesos slaves, but dont at the moment

https://github.com/mesosphere/kubernetes-mesos

interesting - kubernetes api implemented in mesos

summary - small team can gain from big company infrastructure
