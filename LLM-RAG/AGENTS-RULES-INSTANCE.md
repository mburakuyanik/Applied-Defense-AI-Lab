# AGENTS.md
- Do not preserve backward compatibility. Remove obsolete paths instead of adding compatibility layers, fallbacks, or migrations.
- Choose the simplest implementation that fully meets the current requirements. Avoid speculative abstractions, configuration, and indirection.
- Grow the system in layers. Start from the smallest version that works end
8
to end, and add each new capability on top of a product that already
9
works. Never trade a working product for unfinished complexity.
10
- Keep components modular and concerns clearly separated.
11 - Prefer established, well-maintained libraries when they reduce overall
12
complexity or improve reliability. Do not reimplement common
13
functionality without a clear reason.
14
- Lean on the dependencies already in the project before writing your own
15
implementation or adding packages. Do not assume a library lacks a
16
capability without checking its documentation and types.
- Make architectural decisions for the long term. Do not accept a stopgap
18
that only works for now and is meant to be replaced later.
