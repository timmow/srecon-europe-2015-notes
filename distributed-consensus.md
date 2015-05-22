# Distributed Consensus Algorithms for Extreme Reliability

consensus - road to true and lasting bliss

good for resiliency

can help avoid split brain / split cluster

group membership - logically the same

reaching agreement among group of processes connected by unreliable comms
network

flp impossibility paper

PAXOS

RAFT

mencius

replicated state machine

queueing is distributed consensus
locking is distributed consensus

Perceived latency varies depending on where master is

new protocols keep switching master to avoid this

quorum, majority of running processes

three dcs, one fails, end up with not enough traffic for distributed system,
hence drills

across dcs, majority quorum not performant

"hierarchical quorum"

"duelling proposers" bad. keep proposing the same thing, gets rejected, can go
on indefinitely.

monitoring -
number of systems up
health / status
mastership changes
transaction id
errors, request latency

http://research.microsoft.com/en-us/um/people/blampson/58-consensus/abstract.html

http://highscalability.com/paper-consensus-protocols-two-phase-commit
