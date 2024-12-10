# Reverse Engineering Challenge

## Challenge Description
A binary file was provided, and the objective was to find the hardcoded password.

---

## Steps to Solve
1. **Analyze the Binary:**  
   - Loaded the binary into Ghidra and decompiled it.  
   - Found a function comparing user input with a hardcoded password.

2. **Extract the Password:**  
   - Identified the password string in the assembly code: `SuperSecret123`.

3. **Test the Password:**  
   - Entered `SuperSecret123` into the application and solved the challenge.

---

## Lessons Learned
- Reverse engineering requires understanding assembly and binary structures.
- Tools like Ghidra and IDA Pro are essential for analyzing binaries.

---
