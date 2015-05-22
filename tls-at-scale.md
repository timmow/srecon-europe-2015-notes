# HTTPS and Forward Secrecy at Scale

everyone has to have A+ ssl rating is incorrect

valid reasons for not having A+

can I cut a revenue source off?

whats harm of not getting A+?

snowden - someone might decrypt traffic

perfect forward secrecy

drop the perfect! - mathematical def of perfect is different

can decrypt with wireshark if you have the servers private key, pfs stops this

RSA very mature, modular arithmetic, easy to accelerate in hardware. - no
forward secrecy

DHE is alternative diffe-hellman ephemeral - ephemeral important part

ECDHE same but different, EC is elliptic curve

EPHEMERAL is single use keys

Discrete logarithm - much harder to accelerate in hardware - accelration is less
mature, will catch up in time.

so today, must pay for forward secrecy 4x - 10x slower. Can be an order of
magnitude slower.

so we need to test. get real numbers, conventional wisdom may be different in
your situation

each phase of transaction, how long client / server took

built a solution that will be open sourced.

more realistic testing

look at logs to determine browser / cipher suite ratio

endpoint to show info about which cipher suite was negotiated

use selenium to query against test cluster

load balancer gave update, including microcode update. - canaried it, safari6
started causing problems.


