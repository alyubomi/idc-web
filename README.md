# Immersive Data Classroom — web build

Compiled build only. The source lives in a private repository.

**Open it:** https://alyubomi.github.io/idc-web/

Built from commit `8740e27` (v0.6) (v0.6).

## What this build is, and is not

It runs the **GL Compatibility** renderer, because that is what a browser
gets. The desktop build runs `forward_plus`. Those two renderers disagree,
and a bug that appears on only one of them is a real thing that has happened
on this project. So this is a faithful test of layout, controls, filters and
data handling — and it is **not** evidence about shaders, point culling, or
anything else the GPU decides.

It is single-threaded (`thread_support=false`) so it can be served from a
plain static host with no `COOP`/`COEP` headers.

Settings persist to browser storage, per browser, and vanish with site data.
