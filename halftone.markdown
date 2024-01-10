---
layout: page
title: Halftone Tutorial
permalink: /halftone/
---

# Halftone Tutorial

Color printing frequently uses fewer colors of ink than there are
colors in the source image. Halftones are often used to fool the eye
into seeing a broader range of colors. Similar to shading in drawing,
halftones create the appearance of varying tones by varying the size
of dots or lines of ink.

For most of us, this is a historical curiousity or an obscure
technical detail, but Pop Artist Roy Lichtenstein celebrated the lowly
halftone by making the dots large. With the advent of PhotoShop, it
became possible for someone without specialized equipment to
experiment with halftones and various other special effects in persuit
of cool images and techniques.

My company logo was one result of my experimentation with image
filters. I've recreated my logo using Gimp so anyone can play along
without expensive software.

The logo is generated algorithmically without drawing a thing.
1. | Fill a square canvas with light gray | 
![Solid gray field](assets/gray-square.png){: width='100'} |

1. | Convert the light gray to dots using the "Newsprint" filter |
[![Polkadots at a 45° angle](assets/polkadots.png){: width='100'}](assets/polkadots.png) |

1. | Use the "Spherize" filter to create the Op Art illusion of depth |
[![Dots distorted into a sphere](assets/raw-spherize.png){: width='100'}](assets/raw-spherize.png) |

1. | Use a circular selection inverted to remove the background from the sphere | 
[![Dot sphere isolated from the background dots](assets/black-dot-sphere.png){: width='100'}](assets/black-dot-sphere.png) |

1. | Adjust the color, size, and format of the image for its intended use |
[![Op art sphere](assets/green-dot-sphere.png){: width='100'}](assets/green-dot-sphere.png) |

There is plenty of fun to be had starting from solid colors, gradients, or noise and applying various distortion filters.

[![Sphere of stripes](assets/stripe-sphere.png){: width='100'}](assets/stripe-sphere.png) [![Whirl applied to a grid](assets/whirl-and-pinch.png){: width='100'}](assets/whirl-and-pinch.png) [![Diagonal linear gradient](assets/diagonal-gradient.png){: width='100'}](assets/diagonal-gradient.png) [![Convex stripes from halftoning a linear gradient](assets/convex-stripes.png){: width='100'}](assets/convex-stripes.png) [![Wavy stripes](assets/convex-stripes-waves.png){: width='100'}](assets/convex-stripes-waves.png) [![Wavy stripes](assets/fractal-trace.png){: width='100'}](assets/fractal-trace.png)
