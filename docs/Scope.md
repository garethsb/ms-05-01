# AMWA NMOS Control Architecture \[Work In Progress\]

{:.no_toc}

- A markdown unordered list which will be replaced with the ToC, excluding the "Contents header" from above
{:toc}

_(c) AMWA 2021, CC Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)_

## Scope and purpose

This document introduces NCA, the **NMOS Control Architecture**. NCA is an architecture for modeling media devices, and controlling and monitoring them over IP networks.

In this and other NCA documents, the term "device control" means "device configuration, control and monitoring" unless otherwise specified. Note that the use of the term "device" in this document does not have exactly the same meaning as it does in earlier NMOS IS-xx specifications. In this document we use the terms "NCA device" and "NMOS device" to make the distinction clear.

NCA's specification is designed to complement and interoperate with the existing family of [NMOS][] specifications, particularly [IS-04][], [IS-05][], [IS-07][], and [IS-08][].

**NCA's purpose is device control (and status monitoring) only.** NCA does not define higher-level mechanisms such as compound media formats, production role data, studio asset records, facilities reservations, accounting data, performance rights data, and so on and on. Such mechanisms might build (in part) upon NCA device control, but their specification is out of NCA's scope.

**NCA takes as a requirement that media control networks might not be connected to the Internet.** The general operation of NCA does not depend on connections to external data or code resources. Manufacturers may choose to supply controllers and/or devices that depend on wide-area connections to libraries, cloud services, and so on, but such choices will be application decisions not mandated by NCA.

**NCA can apply equally to physical or virtual NCA devices.** In NCA documentation, the term NCA device refers to both unless otherwise stated.

**NCA is not a device or controller implementation specification.** NCA's features and structures serve to define NCA device Application Programming Interfaces (APIs) that can be used for device control, but the internal programming structures behind those APIs are strictly out of NCA's scope.

**NCA is not a user interface specification.** The NCA control model defines numerous elements with application functions (switches, indicators, gain controls, etcetera), but these elements are embodied only as abstractions in a NCA device control model. How, whether, or when they are represented in a user control interface is out of NCA's scope.

## NCA Documentation Structure

Documentation of the NCA is organized across multiple parts:

1. An **architectural framework** that describes NCA's various models, mechanisms, and rules.
2. A **control repertoire specification** that defines NCA's specific underlying elements for controlling and monitoring the various components of media devices.
3. One or more **protocol specifications** that define protocols for accessing NCA's control features over the network.

In addition to the above, NCA anticipates that future phases of work will develop processes for the documentation and curation of a growing set of common models and mechanisms for typical devices and device components found in practice. By leveraging these common models and mechanisms, interoperability between control systems and devices can be improved, and custom engineering avoided in many cases..

### Scope of this document

This document describes the NCA architectural framework - item (1.) in the preceding section. The subsequent documents will be developed in later phases of the NCA workstream.

## References

<!--
[AS-10]: https://static.amwa.tv/as-10-mxf-for-production-spec.pdf "AMWA AS-10 MXF for Production"

[BCP-003-01]: https://specs.amwa.tv/bcp-003-01 "AMWA BCP-003-01 Securing Communications in NMOS Systems"

[BCP-003-02]: https://specs.amwa.tv/bcp-003-02 "AMWA BCP-003-02 Authorization in NMOS Systems"

[BCP-003-03]: https://specs.amwa.tv/bcp-003-03 "AMWA BCP-003-03 Certificate Provisioning in NMOS Systems"

[INFO-002]: https://specs.amwa.tv/info-002 "AMWA INFO-002 NMOS Security Implementation Guide"
-->

[IS-04]: https://specs.amwa.tv/is-04 "AMWA IS-04 NMOS Discovery and Registration Specification"

[IS-05]: https://specs.amwa.tv/is-05 "AMWA IS-05 NMOS Device Connection Management Specification"

[IS-07]: https://specs.amwa.tv/is-07 "AMWA IS-07 NMOS Event & Tally Specification"

[IS-08]: https://specs.amwa.tv/is-08 "AMWA IS-08 NMOS Audio Channel Mapping Specification"

<!--
[IS-10]: https://specs.amwa.tv/is-10 "AMWA IS-10 NMOS Authorization Specification"
-->

[NMOS]: https://specs.amwa.tv/nmos "AMWA Networked Media Open Specifications"


AMWA specifications and documents are referenced by hyperlinks.

IETF RFC documents are referenced by constructs of the form **\[RFC n\]** where n is the RFC number.