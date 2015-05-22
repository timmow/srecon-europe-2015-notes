# Debugging and Extending Distributed Coordination Systems

zookeeper

maintaining / propogating config
distrbuted sync


battle tested
well maintained recipes

bad -

session handling hard
thundering herds
apps can bloat number of watches / reads /writes

configs, services, locks


open question - do all 3 need the same consistency model?

zookeeper needs pings every 1/3 second

services - endpoint is here, doesnt say it is healthy

updates are expensive

locks  - when to release? disconnect or explicit session end?

twitter push it to its limits

https://kazoo.readthedocs.org/en/latest/

running on the bleeding edge - trunk + patches

local sessions are a good feature - dont need to get quorum for as much stuff

zktraffic to analyze zookeeper
