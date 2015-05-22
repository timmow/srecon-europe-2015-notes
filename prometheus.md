# Prometheus: A next gen monitoring system

souncloud originally monolithic rails app, now microservices

built an in house scheduler, random assignment of services

prometheus built to monitor this

2012 - service and host monitoring - statsd / graphite

implicit dimensions in graphite metrics names, not ideal

graphite not good scalability wise

also used nagios

multi dimensional data model - store a metric with multiple values rather than
just one

operational simplicity - go app

scalable data collection - pull not push, simpler to operate / scale

query language, kind of sql like, no logic on client, ask questions later

expression browser looks interesting, has graphing

but promdash is prettier dashboarding

instrument code with client libraries

exporters collect data and export to prometheus

