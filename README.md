# SMPTE _ST 2136-10_ - _Common LUT Format - Broadcast Profiles - Real-time 10-bit Video_

## General

This repository tracks ST 2136-10 Common LUT Format - Broadcast Profiles for Real-time Video Processing

_This repository is *public*._

Please consult [CONTRIBUTING.md](./CONTRIBUTING.md), [CONFIDENTIALITY.md](./CONFIDENTIALITY.md), [LICENSE.md](./LICENSE.md) and [PATENTS.md](./PATENTS.md) for important notices.

Your feedback is welcome at <https://github.com/SMPTE/st2136-10/issues>.

## First Public Committee Draft (PCD1) Notice

The first Public Committee Draft (PCD1) of ST 2136-10 is made available in
10e-st-2136-10-cd-2026-04-02-draft.zip for a review period ending no later than
2026-05-05.

To view the document, please download the
[ZIP file](./10e-st-2136-10-cd-2026-03-31-pub.zip), extract the files, and
open the HTML file in your browser.

## General

This project creates profiles of the new SMPTE Standard ST 2136-1 Common LUT Format for use in real-time, live video production.

Comments are invited and should be recorded at: <https://github.com/SMPTE/st2136-10/issues>.

In high-end modern live television production, there is often a need to produce a number of output formats for delivery to the end user, to other broadcasters and to the archive.  When producing multiple video formats, broadcasters and production companies currently rely on Look-up Tables (LUTs) to perform a range of conversions.  Current LUT formats can be difficult to use and require expert knowledge to install correctly.

SMPTE ST 2136-10 aims to make the process much easier:

  * The specification limits the allowable CLF ProcessNodes and their order to ensure that these hardware-friendly CLFs are easy to implement,

  * The CLF contains machine-readable metadata describing the input and output video formats allowing the hardware to correctly choose matrix parameters, correctly signal the output format and check the input format,

  * The CLF contains a number of human-readable descriptions of the processing undertaken and the input and output formats.  Multiple language versions of these descriptions can be stored, permitting manufacturers to offer a choice to the user.

  * Additional keywords can also be stored which can be used within a GUI to explain to the user what the transform is designed to do. 

  * Unlike previous LUT formats, only one file is required to handle both full- and narrow-range video formats with the logic processing required standardized.  When processing narrow-range video signals, above nominal white and below nominal black signal levels are maintained.

  * Similarly, the specification describes how a single file can be used for different bit-depth videos.

  * Each process has a unique ID and the ability to store the ID of the recommended inverse transform, this allows simplified "round-tripping."

  * The output video clipping can be defined, and clipping can be applied to protect SDI timing words or to be compliant with recommendations such as EBU R103.

  * Failure handling is also defined so that, when an issue occurs, a known failure state will be encountered.

  * Recommended C2PA metadata is provided.

  * Finally, informative annexes discuss the terminology that has come in to use in live, multi-format production.  Descriptions and definitions are given for LUT types, display-light and scene-light mapping between formats, up-mapping, down-mapping, direct-mapping and type-conversion

**Implementers are encouraged to review the system and provide feedback as soon
as possible but no later than May 05, 2026, via GitHub, to help improve the
document and enhance interoperability across implementations.**

## Reporting issues

Please report issues at <https://github.com/SMPTE/st2136-10/issues> or to 10E
Chairs <10e-chair@smpte.org>.

## Contributing

The draft version(s) of this document is accessible to SMPTE Standards Community
members at <https://github.com/SMPTE/st2136-10-private>.
