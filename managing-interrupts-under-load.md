# Bad Machinery— Managing Interrupts Under Load

interrupts - tactical immediate fixes

not fun

at google, pages -> primary, tickets / interrupts to secondary oncall

in practice, tickets / interrupts go to everyone, not just the secondary,
because need to determine if it should go to the secondary

if there are too many interrupts for these 2 people, breaks down

some interrupts are specialised to one person, subset of team

ticket comes in, round robin assigned - this is stupid! (basically 2ndline?)

antipatterns

   - the gauntlet - oncall for a week, forget when not oncall - nothing ever
     gets fixed
   - busy worker - people will do tickets because they enjoy thing, feel like
     they can be sucessful. failure of manager. not good long term
   - amazing disappearing category - set of tickets only one person looks at

context switches are hard.

oncall is a project - needs to evolve over time

fairness is easy to program - if you assume people are machines

dont have instant context switch capabilities

"humans are bad machinery"

"cognitive flow is precious" - most teams attribute no value

"time should be polarised - do one thing well"

when on call, expected not to work on any projects at all

dont use email alerts

policy is as powerful as code - dont try and use code to solve everything when
changing behaviour can work

make sure you agree with the right people the parameters for oncall - time to
respond to page, how many 9s

minimise time individual can be interrupted

do for interrupts what you do for oncall

respect customer and respect yourself.
