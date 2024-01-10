---
layout: page
title: Patents
permalink: /patents/
---

# Patent Portfolio of John D. Corbett

Patents help protect corporations by raising the barriers to entry for
would-be competitors and by providing a defense against accusations of
intellectual property infringement. Over the years, I've had the
pleasure of authoring or co-authoring ten patents. Although most of
them are in the area of Electronic Design Automation, that's because
Xilinx was particularly supportive of inventors and I spent over a
decade there. My first and one of my best is in the area of user
interface development.

Patents are written using a particular style and jargon. I've
attempted to describe my patents here in plain language, so even if
you're not a specialist, the gist of each should make sense.


## Electromagnetic Verification of Integrated Circuits
[US 10107855 · Issued Oct 23, 2018](https://patents.justia.com/patent/10107855)

One aspect of securing cryptographic equipment is detecting when
tampering has occurred such as a part substitution during
manufacturing. Another aspect is preventing sensitive information from
leaking via side-channels such as changes in power consumption or
radio emanation.

It occurred to me that recording radio emanations near an integrated
circuit (IC) could be used as a baseline to detect future
tampering. The emanation could be turned into a digital fingerprint
specific to the IC and the computation it was performing. If at some
later time, the IC was replaced with a counterfeit, a second
measurement would differ from the first revealing this. This technique
could be used to reduce supply chain risks.


## Method and circuits for superclocking
[US 9436786 · Issued Sep 6, 2016](https://patents.justia.com/patent/9436786)

In modern integrated circuits, heat dissipation is often the limiting
factor on performance. As we move to ever smaller transistors, the
amount of so-called "dark silicon" that cannot be used due to thermal
constraints increases. The gist of this invention is to spread the
heat around the IC by moving computations among redundant functional
units. Before one part of the IC overheats, the computation is
transferred to another cooler part, thus enabling the IC to run
faster than it would if limited by the single hotest region of the
IC.

## Prioritized detection of memory corruption
[US 8522091 · Issued Aug 27, 2013](https://patents.justia.com/patent/8522091)

A field-programmable gate array (FPGA) is general purpose integrated
circuit that are configured to perform a specific computation by
setting control registers and defining signal paths between functional
units. The configuration is a binary sequence called a bitstream. The
bitstream is read into the device sequentially and subsequently
resides in the configuration memory of the FPGA.

For applications requiring high reliability, it is important to
monitor and correct application memory and configuration memory
because cosmic rays or high energy protons can cause memory cells to
flip at random thus changing the circuit or changing the state of the
circuit.

The process of correcting configuration memory is commonly performed
in a repeated sequential scan with each configuration memory element
being repaired at the same rate as the others. However, with analysis,
it is possible to learn which elements of configuration memory are
more likely to result in malfunction if randomly flipped. The gist of
this invention is to scan the more critical configuration memory
elements at higher frequency than the rest to reduce the risk that a
random memory flip will affect an ongoing computation.

## Reducing susceptibility of circuit designs to single event upsets
[US 8065644 · Issued Nov 22, 2011](https://patents.justia.com/patent/8065644)

My first role at Xilinx was to take over maintenance of a design tool
for FPGA application developers working on satellite applications. The
tool was used to add triple modular redundancy to a given design. When
it was not practical to triplicate the entire design, the designer
would selectively triplicate portions of the design.

Using fault injection, it was possible to discover which parts of a
design were most likely to fail in the presence of a fault.

Combining these two ideas would allow the design mitigation choices to
be automated.

## Isolation verification for implementing modular redundancy within programmable integrated circuits
[US 8065642 · Issued Nov 18, 2011](https://patents.justia.com/patent/8065642)

When using modular redundancy to improve reliability, it is important
to minimize or eliminate single points of failure that corrupt
multiple redundant modules. Most of my career at Xilinx worked on
design verification tools that would analyze and report portions of a
design that could potentially allow a single fault to corrupt multiple
modules. The gist of this patent is to use isolation verification
methodology to assess the robustness of modular redundancy.

## Isolation Verification within Integrated Circuits
[US 7949974 · Issued May 24, 2011](https://patents.google.com/patent/US7949974)

After WWII, cryptographic equipment in the US and the UK was not
permitted to have information from multiple levels of classification
in a single circuit. This simplifies the analysis of ways information
might unintentionally leak from one part of the system to another.

As integrated circuits grew, this restriction became increasingly
onerous. I was part of a team that collaborated with US and UK
intelligence agencies to modernize the requirements for cryptographic
equipment. My contribution was to create analysis tools that would
show the specific extent to which modules within a single FPGA
integrated circuit were isolated from each other.

This patent describes how we analyzed the designs. There were two
approaches. The first was to search for routes between modules that
could be constructed by assuming a given number of faults could
occur. The second method used the tile-based layout of the FPGA to
examine a barrier of inactive tiles between modules.

## Methods for automatically generating fault mitigation strategies for electronic system designs
[US 7930662 · Issued Apr 19, 2011](https://patents.justia.com/patent/7930662)

There are several techniques for mitigating faults including modular
redundancy, error correcting codes, temporal redundancy, etc.  This
patent emphasizes selection among various mitigation techniques as a
way to automate fault mitigation in a circuit design.

## Verifying design isolation using bitstreams
[US 7797651 · Issued Sep 14, 2010]/patents.justia.com/patent/7797651)

Xilinx had tools for generating and combining partial FPGA
configuration bitstreams where each bitstream would contain one or more
modules. Xilinx also had tools for injecting faults in the
configuration memory resulting from a bitstream and mapping the fault
location to a specific circuit element. The gist of this patent was to
treat bitstreams as sets of components and intersect the sets to find
common elements representing potential single points of failure.

## Generic transfer of exclusive rights
[US 6161121 · Issued Dec 12, 2000](https://patents.justia.com/patent/6161121)

This patent describes a protocol for a transfer of digital access via
an automated escrow agent. My contribution was to propose blinding the
escrow agent to the digital assets being transferred.

## Interactive method of developing software interfaces
[US 5041992 · Issued Aug 20, 1991](https://patents.justia.com/patent/5041992)

Nowadays we take for granted computer graphic computer displays with a
pointing device (typically a mouse or touchpad) and graphic objects on
the display that can be clicked, selected, and dragged with the
pointing device. When this patent was written, these ideas were
new. The prevailing paradigm for building graphical interfaces was to
write program code to draw on the display, to read the pointing
device, and to update the display based on the users actions with the
pointing device, and the keyboard.

My group was developing direct manipulation interfaces that relied on
selecting and dragging graphical objects around the display. I
realized we could save time if instead of building each interface from
new program code, we had an graphical tool for building graphical
interfaces and an interpreter for running the interface. A drawing
program was integrated into a generalize system for dragging graphic
objects around the display. A graphic object could have an associated
map labeling various parts of the object for specialized interaction
such as buttons or connection points. The program code associated with
a clicking on a part of the object could be accessed for editing by
holding a modifier key while clicking it, so the programmer would not
even need to know the name of the part in advance. We build a direct
manipulation user interface for building direct manipulation user
interfaces.

Later, Apple HyperCard, NeXT Interface Builder, Microsoft Visual Basic
and others would implement similar ideas.

