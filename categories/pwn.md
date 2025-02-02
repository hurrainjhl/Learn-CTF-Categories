# Pwn (Binary Exploitation) in CTFs

Becoming proficient in **pwn (binary exploitation)** for Capture The Flag (CTF) competitions is a challenging but rewarding journey. This guide provides a step-by-step roadmap for beginners to become experts in binary exploitation.

---

## Table of Contents
- [Phase 1: Build Your Foundations](#phase-1-build-your-foundations)
- [Phase 2: Learn Binary Exploitation Basics](#phase-2-learn-binary-exploitation-basics)
- [Phase 3: Intermediate Exploitation Techniques](#phase-3-intermediate-exploitation-techniques)
- [Phase 4: Advanced Techniques](#phase-4-advanced-techniques)
- [Phase 5: Practice Makes Perfect](#phase-5-practice-makes-perfect)
- [Phase 6: Advanced Knowledge](#phase-6-advanced-knowledge)
- [Phase 7: Share and Contribute](#phase-7-share-and-contribute)
- [Resources](#resources)

---

## Phase 1: Build Your Foundations

### Understand Basic Programming Concepts
- Learn **C**: Most binary exploitation revolves around vulnerabilities in C programs.
  - Focus on pointers, memory management, and buffer handling.
- Learn **Assembly Language**:
  - Understand how high-level code translates to assembly.
  - Focus on x86/x64 architecture.

**Resources**:
- "The C Programming Language" by K&R.
- Online x86 Assembly tutorials (e.g., [opensecuritytraining.info](https://opensecuritytraining.info/)).

### Learn How Computers Work
- Understand computer architecture:
  - CPU registers (EAX, EBX, etc.).
  - Stack, heap, and memory layout.
  - Endianness (little-endian vs. big-endian).
- Operating systems:
  - Learn the basics of Linux: file permissions, processes, system calls.
  - Explore ELF (Executable and Linkable Format) files.

**Resources**:
- "Computer Organization and Design" by Patterson and Hennessy.
- TutorialsPoint: Linux tutorials.

---

## Phase 2: Learn Binary Exploitation Basics

### Understand Common Vulnerabilities
- **Buffer Overflow**:
  - Stack-based: Overwriting return addresses.
  - Heap-based: Exploiting dynamic memory allocations.
- **Format String Vulnerabilities**.
- **Integer Overflow/Underflow**.
- **Use-After-Free (UAF)**.
- **Double-Free**.

**Resources**:
- [OWASP Binary Exploitation](https://owasp.org/).
- "Hacking: The Art of Exploitation" by Jon Erickson.

### Practice Basic Exploits
- Write simple vulnerable programs to exploit:
  - Overwrite return addresses.
  - Modify variables in memory.
- Use **gdb** (GNU Debugger) to analyze program behavior:
  - Learn breakpoints, stepping through instructions, and examining memory.

**Tools**:
- `gdb` (or `pwndbg` for enhanced debugging).
- `objdump`, `strings`, and `readelf` for binary analysis.

---

## Phase 3: Intermediate Exploitation Techniques

### Learn About Protections
- **ASLR** (Address Space Layout Randomization): Understand how to bypass.
- **NX/DEP** (No eXecute/ Data Execution Prevention): Introduce Return-Oriented Programming (ROP).
- **Stack Canaries**: Identify ways to leak or bypass them.
- **PIE** (Position-Independent Executables).

### Learn ROP (Return-Oriented Programming)
- Craft ROP chains to execute arbitrary code even when the stack is non-executable.
- Use tools like ROPgadget or ropper.

**Resources**:
- [ROP Emporium](https://ropemporium.com/).
- Exploit Education.

### Understand Shellcoding
- Write custom shellcode in assembly.
- Use tools like `nasm` to assemble your shellcode.
- Learn how to encode/pack shellcode to bypass filters.

**Resources**:
- "Shellcoder's Handbook" by Koziol et al.
- Online shellcoding tutorials.

---

## Phase 4: Advanced Techniques

### Heap Exploitation
- Learn about heap management in libc (e.g., `malloc`, `free`).
- Understand **fast bins**, **unsorted bins**, and other heap structures.
- Explore heap exploitation techniques (e.g., House of Spirit, House of Force).

**Resources**:
- [Heap Exploitation](https://heap-exploitation.dhavalkapil.com/).
- Research on modern heap attacks.

### Learn Exploitation Frameworks
- Automate your exploits using **pwntools** (Python library).
- Practice building robust scripts for exploitation.

**Tools**:
- Pwntools.
- Libc-database (find the right libc version for exploits).

### Kernel Exploitation (optional, advanced)
- Study kernel memory structures.
- Learn how to exploit kernel bugs (e.g., privilege escalation).

---

## Phase 5: Practice Makes Perfect

### Practice on Vulnerable Programs
- Platforms for binary exploitation:
  - [Pwnable.kr](http://pwnable.kr/): Beginner to advanced challenges.
  - [CTFlearn](https://ctflearn.com/): Beginner-friendly.
  - [Exploit Education](https://exploit.education/): Focused labs.
  - [OverTheWire (Narnia)](https://overthewire.org/wargames/).

### Participate in CTFs
- Join CTFs with a focus on binary exploitation.
- Platforms:
  - [CTFTime](https://ctftime.org/): Ongoing CTFs.
  - [Hack The Box](https://www.hackthebox.com/): pwn-focused challenges.

---

## Phase 6: Advanced Knowledge

### Modern Exploit Development
- Learn about modern OS exploitation techniques.
- Study bypasses for modern mitigations (e.g., CFG, Shadow Stacks).

### Reverse Engineering
- Master tools like IDA Pro, Ghidra, and Binary Ninja.
- Combine reverse engineering with exploitation.

---

## Phase 7: Share and Contribute
- Write your own CTF write-ups for binary challenges.
- Contribute to tools and resources in the security community.

---

## Resources

### Tools
- **GDB**: [GDB Official Website](https://www.gnu.org/software/gdb/)
- **Pwntools**: [Pwntools GitHub](https://github.com/Gallopsled/pwntools)
- **ROPgadget**: [ROPgadget GitHub](https://github.com/JonathanSalwan/ROPgadget)

### Learning Platforms
- [Pwnable.kr](http://pwnable.kr/)
- [CTFlearn](https://ctflearn.com/)
- [Exploit Education](https://exploit.education/)

### Books
- **"Hacking: The Art of Exploitation" by Jon Erickson**: A comprehensive guide to binary exploitation.
- **"Shellcoder's Handbook" by Koziol et al.**: A deep dive into shellcoding and exploitation.

### Communities
- [Reddit r/netsec](https://www.reddit.com/r/netsec/)
- [CTFtime](https://ctftime.org/)

---

Binary exploitation is a challenging but rewarding skill in CTFs. Start with the basics, practice consistently, and gradually move into advanced topics like heap exploitation and kernel exploitation. Happy hacking! 🚀
