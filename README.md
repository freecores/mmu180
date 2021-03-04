# mmu180
MMU for Z80 and eZ80

_Originally created 2013-10-05 on opencores.org_

#### Description
mmu180 is a MMU (memory mananagement unit) designed per original specifications of Zilog's Z180 family of processors (including Hitachi HD64180), which can be used to enhance any Z80-compatible core or physical processor to address up to 1 MiB of memory, per the original MMU specification. It allows most software written for Z180 devices to run on either a Z80-compatible core with mmu180, or on an actual Z80 or eZ80-family processor interfaced to mmu180 (e.g. in CPLD).

#### Status
At present, has been simulated with Icarus Verilog and also from within Xilinx ISE WebPACK, and was successfully fitted into a Xilinx XC95144XL CPLD.

Actual validation of the MMU180 design is slated to proceed on a Zilog eZ80L92-based prototype. However, the challenge remains to obtain known working source code which can both reliably detect the presence of a Z180 MMU, and then run a comprehensive memory test suite to validate that the MMU functions properly "in situ". Beyond this, the design could be further and fully validated with confidence by running an operating system such as a version of CP/M Plus or Z-System which utilizes a Z180-compatible BIOS.
