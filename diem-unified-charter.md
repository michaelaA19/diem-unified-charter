# Terminology

Bearers: assets of any kind that have digital emblems associated with them for
    Verifiers to discover.

Responsible Entities: entities that are responsible for the development of the
    distinctive emblems under International Humanitarian Law. These may be
    elsewhere known as legal guardians, depositories, or other things depending
    on the Responsible Entity.

Verifiers: parties that check potential Bearers for the presence of digital
    emblems.

# Use Cases

Digital emblems is a catch-all term for mechanisms that convey information
of legal, compliance, or other significance associated with a Bearer that need
to be verified and should inform some behavior of Verifiers. These use cases are
broken down into categories based on similarities in requirements and whether
the use cases have Responsible Entities that determine the fitness of a given
technical solution. While emblem format is expected to maximize reuse, emblem
discovery and conveyance mechanisms result in the divergent requirements that
motivate these categories.

## Digital Protection with Responsible Entities

This category includes use cases for digitally signaling an emblem to inform
Verifiers that digital attacks against the Bearer are forbidden by law.
Verifiers may not ever interact with the Bearer in a physical manner, so there
is no concept of binding this emblem to a physical object.

These emblems have legal guardians that determine whether a given technical
solution is acceptable for their use case(s). Known use cases include the Blue
Shield (UNESCO) and Red Cross/Crescent/Crystal (ICRC).

Unique technical requirement(s):
- must prevent Bearers from discovering Verifiers
- must meet requirements of legal guardians to be useful to implementors

This work is recommended for a new WG based on the first requirement not
existing in any current WG charter. It is expected that the format of the
emblems will be coordinated with other WGs to maximize reuse.

## Physical Protection with Responsible Entities

This category includes use cases for digitally signaling an emblem to inform
Verifiers that physical attacks against the Bearer are forbidden by law.
Verifiers primarily interact with the Bearers physically, so the digital
emblem must be verifiably bound to the physical asset and discoverable through
digital means that are achievable via physical proximity or use of information
discovered through physical observation.

These emblems have Responsible Entities that determine whether a given technical
solution is acceptable for their use case(s). Known use cases include the
labeling protected members of the press (???Resp. Entity???), TODO: others?

Unique technical requirement(s):
- must be bound to and discovered for a physical Bearer
- must meet requirements of legal guardians to be useful to implementors

This work is recommended for adoption by SPICE based on the "physical binding"
requirement's similarity to SPICE use case 5.2 [1]. It is expected that the
format of the emblems will be coordinated with other WGs to maximize reuse.

## Physical Properties with or without Responsible Entities

This category includes use cases for digital discovery of mutable information
bound to a physical object. Unlike the other categories, this category enables
the digital discovery of variable and mutable data that is bound to a physical
object without association to a protected legal status (even if the emblem
itself is legally defined).

These emblems may not have Responsible Entities, so defining an acceptable
solution may be up to consensus among implementors (as is typical in the IETF).
Known use cases include ISO labels on packages, TODO: others?

Unique technical requirement(s):
- must be bound to and discovered for a physical Bearer
- must support mutable data such as Bearer access logs or content changes

This work is recommended for adoption by SPICE based on the "physical binding"
requirement's similarity to SPICE use case 5.2 [1]. It is expected that the
format of the emblems will be coordinated with other WGs to maximize reuse.

# Pre-existing Work

There are existing digital emblem solutions today, such as the Whiteflag
protocol, that new and existing WGs are recommended to use as working examples
that may prove useful during solution design (whether or not these existing
solutions can be directly reused).

# Note on Responsible Entities

It is not typical for IETF work to address the expectations of Responsible
Entities for a standard to be considered fit for its purpose. Chartered work
for use cases with legal guardians should only adopt scope and develop solutions
for Responsible Entities who are actively engaged (in addition to the typical
engagement of future implementors) to avoid inventing solutions that will not be
adopted by their intended audience.

# References

[1] https://datatracker.ietf.org/doc/draft-ietf-spice-use-cases/
