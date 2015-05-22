# How Container Clusters Like Kubernetes Change Operations

decoupling SRE

	hardware
	kernel / os
	cluster
	application


unified compute substrate

pod is collection of one or more containers, share filesystems / namespaces

example - one container to watch git repo, another to nginx

another example - one container prometheus statsd bridge, one container has
webapp. webapp can talk to bridge on localhost

combining containers into single atomic unit

labels - kv pairs describe containers

stage:production, role:backend

no hierarchy, label queries to group them to service different things

replication controller - cookie cutter to build out a stack.

takes care of scaling up / down, health check

services - combining service discover with automated maintenance

example - frontend needs to talk to backend - services allow a fixed ip address
for backend, so frontend doesnt need to care where backend is

example - 3 apps running, one fails - trad approach to kill the failing one, but
likely not enough logs. labels help - can remove production label when failing.
replcation controller will spin up a new app because labels dont match, will
also be removed from lb. developer can look at remaining running sick pod

demo of a rolling update - creates a new replication controller, traffic
balanced across old and new controller. when all updated, old pods destroyed
adds one new, removes one old, until all replaced.

decoupling the network

containers have own ip addresses

layer software defined network on top of containers. routing is problem of SDN
