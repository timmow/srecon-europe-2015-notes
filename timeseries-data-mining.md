# Signatures, Patterns, and Trends: Timeseries Data Mining at Etsy

kale, skyline and oculus

needs to be realtime

turned out to be more difficult than expected

now not using it internally, noone is using it outside of etsy

still an unsolved problem, we dont have a working solution

twitter / netflix just released packages, yahoo have a dataset for benchmarking

kale 1.0 - what worked well?

timeseries similarity search

done using elasticsearch hack - map line segments to tokens based on gradients,
do a sloppy phrase query in elasticsearch!

what was hard?

complex architecture - python + ruby + java + js. redis + elasticsearch. flask +
sinatra...

anomaly detection was tricky

distributions assumed to be normal, were not

spikes + periodic cycles

lots of false alarms

not every anomaly is point outlier

need to take into account lots of context

periodic oscillations can sometimes appear from nowhere, or disappear


