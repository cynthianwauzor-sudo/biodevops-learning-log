# Day 2: Automating Security with Bash
Date: 2026-01-14

**The Challenge:**
Manually securing patient data is slow and error-prone.

**The Solution:**
I wrote a Bash script (`setup_lab.sh`) that accepts a disease name as a variable (`$1`) and automatically:
1. Creates a dedicated directory.
2. Generates the patient file.
3. Locks permissions to `600` (Owner Read/Write only).

**Code Snippet:**
```bash
echo "mkdir -p experiment_data" > setup_lab.sh
echo "touch experiment_data/\$1.dna" >> setup_lab.sh
echo "chmod 600 experiment_data/\$1.dna" >> setup_lab.sh
