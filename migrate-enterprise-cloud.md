# Infrastructure Kata and Moving a Large Enterprise to the Cloud

yelp were all hardware "bear metal"

lots of problems, solution was cloud

kata - practice a routine - hone skill through practice repitition

code katas are an example

need a procedure, write down everything you do - you wont write down everything

now you have a procedure - something you can work through

identify weak points, address the worst

have someone else practise it

eventually you get to a single command

so now see how yelp did that for aws migration

packer to bake AMIs

netflix asgard for managing deployments

kata - launch an instance

it is a single command using aws cli tools, but loads of magic numbers /
boilerplate so its not really

so you will end up wrapping it

kata - set up a search server

each host class can be a kata

WRITE EVERYTHING DOWN

iterate until independent

monitoring - originally all done by hand

nagios didnt work for dynamic config

so used sensu, configured with puppet

load balancer config was generated from script

edits and then manual application

but now use airbnb smart stack

first for internal lb, then external lb

test framework called seagull, built on marathon, will be open sourced soon

the future - terraform

katas for building environments

treat each repetition as a practice opportunity

dont despair if stuck with clunky app
