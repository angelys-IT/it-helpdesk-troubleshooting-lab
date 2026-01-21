# Ticket 001 — VM Startup Failure (Aborted State)

**User:** Angelys L.

## Issue
Failed to load the VM, aborted state
## Symptoms
- Aborted state
- Did not boot
- Error text: Failed to load R0 module VMMR0.r0 VERR_LDR_IMPORTED_SYMBOL_NOT_FOUND
## Questions Asked
- What did you see on the screen? 
- Did it boot at all?
- Any error text? 
- When did this start? 
- Does this happen every time?
## Troubleshooting Steps
- Attempted to start the VM and confirmed the aborted state
- Reviewed the error message shown
- Checked VM settings to confirm the correct ISO and hardware configuration
- Reviewed Windows Security settings on the host system
- Disabled Memory Integrity
- Restarted the host system
## Resolution
- Disabled Memory Integrity in Windows Security
- Restarted the host system
- Successfully started the VM
- Started the Windows 11 installation
## What I Learned
VM rely on system drivers that can be blocked by Windows security features, error messages can help identify if an issue is related to the VM or the host, making small, controlled changes can help resolve system level problems.
## Evidence (Existing Repo Folders)
- VM Creation: ../vm_creation/
- Errors: ../errors/
- Fixes: ../fixes/
- Windows Installation: ../windows_installation/
