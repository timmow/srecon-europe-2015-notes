# Perimeter Management at Spotify

spotify - mostly stateless microservices

7k servers, 4 dcs

managed by firewall rules, manually, no audit or overview of what is allowed in

wanted an automated system, devs could use, secure by default, HA, horizontal
scaling

use dyn to direct to healthy, closest dc

devs can just pr a repo, does everything including ssl!

use haproxy to do health checks, can use 3rd party nginx mod or commercial
version

outbound proxy, only http(s) allowed by default
everything else whitelisted, logged
