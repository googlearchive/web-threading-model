At BlinkOn 3, we introduced [Midnight
train](http://bit.ly/blink-midnight-train), which is a set of performance goals
we wish for all web content to be able to achieve on mobile devices. In its
simplest form, we hope that plain old web content can: * Get to a loaded and
interactive state in less than 1000ms on a warm load * Respond to touch down
events within 100ms Maintain 60hz framerate throughout * any interaction or
transition that results Do cleanup/fingerup/idle work in * less than 100ms
chunks so that if a finger down happens again, there will be * only minor lag
returning to a 60hz state.

Careful and judicious use of threads is an essential part of achieving this
goal. Precisely how, we are not sure: maybe it should be possible to write more
declarative touch interactions that can be accelerated by the browser. Maybe
some of the existing compositing machinery should be made
[extensible](https://extensiblewebmanifesto.org/) so that its behavior can be
used by applications. Maybe something else.

We want to throw around requirements, ideas, and dreams in this space, and do so
as openly as possible. This repo is our inital dumping ground for ideas.
