# TryHackMe | The Brochure - Hacker Holidays Day 0

**Room:** hh-thebrochure-081f3e36
**Track:** Hacker Holidays Storyline: Act 0 - Recon
**Category:** OSINT
**Status:** Completed - 100%

### Overview
The Byte Lotus Hotel - The Brochure. First recon task for Hacker Holidays 2026.

### Methodology
1. Opened the brochure PDF / image provided in the room
2. Found hidden Base64 string in the brochure file
3. Used CyberChef (From Base64) and Python to decode
   - Tool: https://gchq.github.io/CyberChef/
   - Command: `echo <string> | base64 -d`
4. Verified flag format THM{...}

### Tools
- CyberChef
- Python base64 module
- TryHackMe AttackBox

### Key Learning
- Base64 encoding is common for hiding data in documents
- Always check file metadata and hidden text in brochures

### Proof
![Room Completed 100%](assets/proof.png)

Completed: 20 Oct 2026
