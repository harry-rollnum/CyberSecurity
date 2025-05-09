# 📘 Linux Terminal Commands - Practical Walkthrough Guide

This notebook summarizes a full hands-on Linux terminal session log. The commands below are categorized and explained to form a beginner-friendly guide for learners to understand Linux basics through terminal exploration.

---

## 📂 Directory Navigation & Creation

### 🔹 Changing Directories

```bash
cd Desktop/           # Move into Desktop
cd Assignment-1       # Enter Assignment-1 directory
cd .                  # Stay in the current directory
cd ..                 # Go up one level
```

### 🔹 Creating Folders

```bash
mkdir Assignment-1                       # Create a directory
mkdir -p Assignment-1/{data,scripts,logs,reports}  # Create folder + subfolders in one go
```

---

## 🌲 Folder Structure Visualization

```bash
tree         # Visualizes folder and file hierarchy
```

---

## 🧹 Deleting Files and Folders

```bash
rm -rf Assignment-1                     # Force delete non-empty folder
rm -ri ./Assignment-1                   # Interactive recursive delete
```

---

## 📄 Creating Files in Specific Folders

```bash
touch data/hello.txt logs/today.txt reports/kamal_report scripts/hello.py
```

---

## 📝 Adding Content to Files

### Using `echo`

```bash
echo "Hello, World!" >> data/hello.txt
```

### Using `cat`

```bash
cat > new.txt         # Adds input (CTRL+D to save)
cat >> new.txt        # Appends input
```

---

## 📜 Reading File Content

```bash
cat data/hello.txt
cat scripts/hello.py
```

---

## 📁 File & Directory Permissions

### Check permissions:

```bash
ls -l
ls -la
```

### Change permissions:

```bash
chmod 700 scripts/hello.py     # Owner: all, others: none
chmod 777 scripts/hello.py     # All permissions to everyone
chmod +x scripts/hello.py      # Make executable
```

---

## 🧑‍💻 Users & Permission Bits

* First 3 bits: **Owner** (e.g., root/user)
* Next 3 bits: **Group**
* Last 3 bits: **Others**

E.g., `-rwxr-xr--` => Owner has rwx, group has r-x, others have r--

---

## 💡 Script Execution

```bash
python scripts/hello.py       # Run Python script via interpreter
./scripts/hello.py            # Run directly if executable (needs shebang)
```

Add shebang for direct execution:

```bash
echo "#!/usr/bin/env python3\nprint('Hello, World!')" > scripts/hello.py
```

---

## 🧾 Logging Terminal Commands

### Save command history

```bash
history > log_today_cmd.txt
```

### Full session recording

```bash
script session_log.txt
exit   # to stop recording
```

---

## 🛠️ Tools Explored

* `mkdir`, `cd`, `rm`, `ls`, `chmod`, `cat`, `echo`, `touch`, `tree`, `script`, `history`

---

## 🎓 Summary

This notebook covers basic Linux terminal skills that are essential for scripting, automation, and system navigation. All commands are practical, tested in a real terminal session, and aimed to help learners develop muscle memory through repetition.

---

## 🔗 Next Steps

* Make this into a GitHub repo ✅
* Add visuals for folder structure (`tree` snapshots)
* Provide tasks/exercises like: "Create your own project layout"
* Add cheat sheet at the end

Let me know if you'd like to generate Markdown or PDF versions!

