# Experiment: Text Searching in Linux Using grep

## Aim
To perform text searching in Linux using `grep`, `fgrep`, and related commands.

## Objective
* To learn searching of text patterns in files.
* To use different `grep` options.
* To understand the difference between `grep`, `fgrep`, and `egrep`.
* To apply text searching in real-world scenarios.

## Theory

### Text Searching in Linux


Linux treats most data as text, making text-processing tools very powerful. Text searching is important for log analysis, troubleshooting, and automation.

### grep Command
The `grep` command is used to search for patterns in files and display matching lines.

**Syntax:**
```bash
grep [options] pattern filename
```

### Related Commands
* `grep` – General pattern search
* `fgrep` – Searches fixed strings (no regex)
* `egrep` – Supports extended regular expressions (`grep -E`)

### Important Options
* `-i` – Case insensitive search
* `-n` – Show line numbers
* `-r` – Recursive search
* `-v` – Invert match

## Step-by-step Procedure

1. **First, logged into the Linux system and opened the terminal.**

2. **Then, created a working directory and moved into it:**
   ```bash
   mkdir grep_lab
   cd grep_lab
   ```

3. **After that, created a sample text file:**
   ```bash
   nano sample.txt
   ```

4. **Then, added the following content:**
   ```text
   Linux is powerful
   Linux is secure
   Bash scripting is useful
   Cyber Security uses Linux
   ```
   *(Saved and exited the editor)*

5. **After that, displayed file contents:**
   ```bash
   cat sample.txt
   ```

6. **Then, searched for a word using grep:**
   ```bash
   grep Linux sample.txt
   ```

7. **After that, performed case-insensitive search:**
   ```bash
   grep -i linux sample.txt
   ```

8. **Then, displayed line numbers with matches:**
   ```bash
   grep -n Linux sample.txt
   ```

9. **After that, inverted the match:**
   ```bash
   grep -v Linux sample.txt
   ```

10. **Then, searched using fgrep:**
    ```bash
    fgrep "Bash scripting" sample.txt
    ```

11. **After that, performed recursive search:**
    ```bash
    grep -r Linux .
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
grep
grep -i
grep -n
grep -r
grep -v
fgrep
cat
ls
```

## Observations / Results
* Matching lines containing the search pattern were displayed.
* Line numbers were shown correctly.
* Case-insensitive search worked properly.
* Inverted search displayed non-matching lines.
* Recursive search worked for multiple files.


## Conclusion
The experiment was successfully completed. Text searching operations were performed using `grep` and related commands. This experiment helped in understanding how to efficiently locate specific patterns in files, which is useful in log analysis, troubleshooting, and automation tasks.
