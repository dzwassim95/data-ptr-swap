# Data PTR Hook Driver

A ready to paste Windows 11 (24H2) kernel‑mode driver that hooks the `NtUserCreateWindowStation` function in `win32k.sys` by swapping its pointer to your function in your mapped driver.

---

## Features

- **Mapped with [Kdmapper](https://github.com/TheCruZ/kdmapper)** 


- **IoCreateDriver (from [Th3Spl](https://github.com/Th3Spl/IoCreateDriver))**  
  Uses `IoCreateDriver` to bypass `PsLoadedModuleList` and `EtwTiLogDriverObjectLoad`.

- **Shared Memory IPC**  
  Creates section objects for fast, secure communication between kernel and user‑mode client.

- **Physical Memory Access**  
  Maps target process physical pages to read/write arbitrary user‑mode memory.

- **Windows 11 (24H2) Support**  
  Tested on Windows 11 version 24H2.

---
