# Continuous Pipelines at Google

progrmams that perform periodic or cont transoforms on data

periodic - cron, start up, do work, shut down

whats wrong -

 * poor monitoring visibility
 * resource exhaustion
 * exceeding runtime deadlines
 * hanging processing chunks

 overlapping problems

 thundering herd problem

 continuous processing at scale

 combination of design patterns, analagous to mvc

 modelled as a series of tasks

  pipeline input injected into roughly equal tasks

  use task master, acid compliant datastore for storing tasks

  mvc

  task master is model, job state
  workers are view, units of work from task master, work on them
  controller / workcycle scaling / snapshotting - not sure exactly

  worker gets a lease with an expiry time, if its not finished, killed
  will drop jobs that have completed with an old configuration

  task master validated as well, multiple task masters, move around, but
  existing job can commit to new task master, thinking it is the old one, so
  force workers to one task master, fail if the worker isnt writing to the
  correct one. 

  uses spanner as a filesystem, spanner is distributed database

cloud dataflow - determines flow graph at runtime

https://cloud.google.com/dataflow/

should switch away from continuous pipeline
