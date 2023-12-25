# Linux commands 

The purpose of this file to collect useful linux commands for reference.

## Copying a broken file

The broken file could contain e.g. CRC (Cyclic Redundancy Check) errors so
ordinary programs/commands will refuse to copy the file.

```bash
 dd if=(sourcefile) of=(targetfile) bs=4M conv=noerror,sync
```
