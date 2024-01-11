---
layout: page
title: Tide Disco
permalink: /tidedisco/
parent: Portfolio
---
# Tide Disco

Success of software projects often depends heavily on ease of use,
both for end users and for developers. Fundamental to easy of use is
making information available where it is needed. This is the goal of
[Tide Disco](https://tide-disco.docs.espressosys.com/tide_disco/).

[Tide](https://github.com/http-rs/tide) is a Rust web application
server. Tide Disco offers a system for adding discoverability to a web
server. Routes and associated documentation are specified in TOML
files loaded at startup. Route parsing is augmented with spelling
correction and error handling that serves context-specific
documentation from the TOML files.

I created the overall design and implemented the discoverability
features. Co-workers helped me with the method for associating route
handlers with routes and support for self-contained API modules to
specify collections of related routes.

Like most things, Tide Disco is a work-in-progress. Ironically, the
code is a bit specialized to the Espresso organization, so not quite
as easy to use as I'd like.

