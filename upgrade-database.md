# Upgrade Your Database without Losing Your Data, Your Perf, or Your Mind

facebook parse - backend as a service

largest and most complicated mongodb deployments, also redis / cassandra

why upgrade, why not, how to?

loads of problems when upgrading dbs

organisational risk, tech risk - maturity, how critical is data?

can you roll back?

minimal process - 

   unit tests
   read release notes
   assess appetite for risk

to do it properly -

  test with real production traffic

  replay queries and compare results - pt-upgrade?

  production traffic splitter

  app connects to splitter, sends query to both, compares, sends prod response
  back to app

  capture / replay

  use lvm snapshots, reset after running test

  be careful you are stressing db, and not replay stuff - monitor the replay
  clients

  be careful when updating clients as well.
