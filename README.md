# Immersive Data Classroom — web build

Compiled build only. Source lives in a private repository.

**Open it:** https://alyubomi.github.io/idc-web/

Built from `v1.0.20+bbfba10`.

## What this build is and is not

It runs the **GL Compatibility** renderer, because that is what a browser
gets. The desktop build runs `forward_plus`. Those two renderers disagree —
a bug that only appears on one of them is a real thing that has happened on
this project. So this build is a faithful test of layout, controls, filters
and data handling, and is **not** evidence about shaders, point culling or
anything else the GPU decides.

It is single-threaded (`thread_support=false`) so it can be served from a
plain static host without `COOP`/`COEP` headers.

Settings persist to browser storage, per browser, and vanish with site data.
