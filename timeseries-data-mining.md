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

trends change, baselines shift - constant growth flatlines

rare discrete events become more frequent or infrequent

all above are signs of something wrong, outlier detection will not pick up

its usually not even a problem

kale 2.0 - phase 1 is thyme

library of algorithms and composable processing steps

reactivex framework

supports flexible experimentation / prototyping.

live demo of recording from microphone, picking up anamolies when clapping and
applause

keep architecture simple

good fit for problem - doesnt mean add to your stack

dont relase platform / product, unless you use it yourself

anamoly detection is more than outlier detection

kale had a good ui
timseries similarity was good
ensemble methods / auto calibration was good


