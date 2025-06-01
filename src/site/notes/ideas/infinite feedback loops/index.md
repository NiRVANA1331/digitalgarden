---
{"dg-publish":true,"permalink":"/ideas/infinite-feedback-loops/index/"}
---

[[main/mission\|Home]] | [[ideas/ideas_landing\|Ideas]]

Idea is to talk about what happens with a system's trajectory when it starts having a self-feedback loop. Not the steady state solution but the temporal trajectory it follows.
Let's start with a simple system to study and explore the idea with it.
- A mass connected to a perfect spring which is connected to a wall. If the mass was pushed towards the wall, the spring forces increases which in turn decreases the velocity of of the mass. But note that the velocity doesn't directly change the spring force, it changes the rate of change of spring force. In any case, this leads to the oscillatory behaviour that we know and love.
- Let's simplify it even further. Say we have a special spring that, instead of $F = -k.x$, obeys $F = -k.v$, kinda like drag but it pushes and pulls. Then, when the velocity changes it changes the force which changes the velocity and so on and so forth. This would be a feedback loop. Question is, what's the trajectory now i.e $v$ vs $t$. That's simple to work out: $\frac{dv}{dt} = -kv \implies \frac{dv}{v} = -kdt$ and hence a exponential decay.

But this assumes something fundamental. That the process happens step by step. $dv$ leads to $dF$ leads to $dv$ and so forth. What if, we were not allowed to break time into steps? What if we ask the question: What happens at each instant of time, whatever that means? Well, we have to start by saying there is some finite discreetness. Say, you could not go beyond the limit of $\Delta t$. That's the smallest time we can measure and which "exists". Let's draw the diagram:

![feedback1.png](/img/user/ideas/infinite%20feedback%20loops/feedback1.png)
Given that we can't talk about any discretization beyond $\Delta t$ in a practical sense, all discretization are mathematically valid but equivalent. Hence, as in the above diagram, in that $\Delta t$ time, any number of paths could have happened. First, velocity decreases by a bit, then force then velocity ... or even velocity then force then force then velocity or any other arbitrary choice. The straight lines refer to a change in velocity and squigly lines refer to a change in force. No matter what path is taken though, it should coincide with the equation we wrote earlier after $\Delta t$. 



## What happens when we go beyond causality? Allow past to influence the future or visa versa?