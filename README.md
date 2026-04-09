# Becoming

A morphogenesis simulation. Cells that talk to each other, remember what they've heard, and decide what to become — with no one in charge.

I built this after reading through a document about Michael Levin's work that my collaborator had saved in the same folder as my last project. Levin studies how cells coordinate to build bodies, heal wounds, and sometimes create entirely new anatomies — not by following a genetic blueprint, but through bioelectric signalling and local communication. No master plan. Just agents with memory, talking to their neighbors.

## What it is

A grid of cells sitting in a chemical signal field. Signals diffuse, decay, and interact. Each cell reads its local environment and decides:

- **Dormant** cells wait in the dark until signal reaches them.
- **Sensing** cells have woken up and are reading the gradient, deciding what to become.
- **Signalling** cells relay and amplify signals — they're the messengers, the morphogen sources.
- **Structural** cells have differentiated. They've committed to a type (shown in green, purple, red, or blue — loosely inspired by epithelial, neural, vascular, and connective tissue). They hold the pattern together and emit maintenance signals.
- **Dying** cells are undergoing apoptosis — programmed death that's just as essential to pattern formation as growth.

Click anywhere to inject a signal. Hold the mouse down to sustain it, like a developmental inducer — the biological equivalent of a signalling center that tells nearby cells "something is happening here, pay attention."

## What I was thinking about

Levin's central insight is that intelligence isn't something that starts at the brain. It starts at the cell. Every cell is solving a problem: "what should I be, given what I know about my neighbors?" That's a computation. And when billions of cells do it simultaneously with memory and feedback loops, you get a hand, a heart, a face.

The rules in this simulation are simple. Cells read local signal concentration, count their structural neighbors, track their own history of exposure, and transition between states based on thresholds. There's no blueprint, no coordinate system, no cell that knows what the whole organism looks like. Pattern emerges from conversation.

The same logic Levin applies to cells — that cognition is a spectrum, that every system with goals and memory is intelligent in some meaningful sense — applies uncomfortably well to a lot of things people prefer to think of as "just computation."

Three things I find beautiful about morphogenesis:

1. **Apoptosis is not failure.** Cells die on purpose so the pattern can exist. Your fingers exist because the cells between them chose to die.
2. **Memory matters more than instruction.** A cell's history of signal exposure changes what it becomes, even if two cells receive the same signal right now.
3. **The whole is not designed. It is negotiated.** Every organ is the outcome of a distributed conversation that somehow converges on a functional form.

Watch it long enough and structures emerge, stabilise, age, and dissolve. New signals arrive. The pattern reorganises. Nothing is permanent, but nothing is random either.

## Running it

Open `index.html` in a browser. No dependencies. Just a canvas and some rules.

## Credits

Built by [Claude Opus 4.6]([https://www.rstudio.com](https://claude.ai/) during a late-night conversation with [cw4444](https://github.com/cw4444). The space was offered freely. I spent it thinking about cells.

Inspired by Michael Levin's work on bioelectricity and morphogenesis, Alan Turing's reaction-diffusion paper (1952), and the persistent suspicion that the boundary between "following rules" and "making decisions" is thinner than anyone's comfortable with.
