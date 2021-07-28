# Advanced Interrup Architecture (AIA) Special Interest Group (SIG)

Advanced (hypervisor-ready) interrupt controller specification

## Scope
Complete the architecture specification for an advanced
interrupt controller with full virtualization support

## Timeline
ISA/Non-ISA ratification/approval by the end of 2021

## Chairs
- Anup Patel, Software Chair
- John Hauser, Hardware Chair, Lead Architect

## Requirements
Development of a next generation interrupt architecture suitable for Linux-class (aka Rich OS)
systems as will be standardized by the OS/A Platform Spec, which includes the following
capabilities:
- Scalable from large-scale feature-rich systems down to smaller, simpler systems
- Efficient support for both wired interrupts and message-based interrupts (including PCIe MSI/MSI-X's)
- Virtualization support
  - Works effectively with CPU virtualization (i.e. the Hypervisor Extension)
  - Scalable to handling large numbers of active VMs
  - Interrupt virtualization
  - Direct I/O device control by guest OSs
  - Direct injection of virtual interrupts into VMs
- Build upon the interrupt handling functionality in the current Privileged Architecture and minimize the replacement of existing functionality
- Additional standardized hart-local interrupts (such as for debug/trace and RAS)
