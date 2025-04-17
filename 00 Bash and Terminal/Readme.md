# Essential Bash Commands Guide 🖥️

A comprehensive guide to fundamental Bash commands for terminal navigation and file manipulation.

## Navigation Commands 🧭

### `pwd` (Print Working Directory)
- Shows the complete path to your current location
- Example: `/home/user/projects`

### `cd` (Change Directory)
- Navigate between folders
- Common uses:
  - `cd ..` → Move up one directory
  - `cd ../..` → Move up two directories
  - `cd ~` → Go to home directory
  - `cd /path/to/folder` → Go to specific directory

### `ls` (List)
- Display contents of current directory
- Useful flags:
  - `ls -l` → Detailed list view
  - `ls -a` → Show hidden files
  - `ls -la` → Combine both flags

## File Operations 📁

### `mkdir` (Make Directory)
- Creates new directories
- Example: `mkdir my_project`

### `touch`
- Creates empty files
- Example: `touch index.js`

### `cat` (Concatenate)
- Display file contents in terminal
- Example: `cat index.ts`

### `cp` (Copy)
- Copy files or directories
- Basic syntax: `cp source destination`
- Example: `cp file.txt backup/`

### `mv` (Move)
- Move or rename files
- Basic syntax: `mv source destination`
- Example: 
  - Move: `mv file.txt documents/`
  - Rename: `mv oldname.txt newname.txt`

## Text Editing with Vi/Vim ✏️

### `vi` or `vim`
- Terminal-based text editor
- Basic usage:
  1. Open file: `vi filename.txt`
  2. Enter insert mode: Press `i`
  3. Exit insert mode: Press `Esc`
  4. Save and exit: Type `:wq!`
  5. Exit without saving: Type `:q!`

## Quick Reference Card 📋

```ascii
+------------------------+
|    Navigation  🧭      |
+------------------------+
pwd → Where am I?
cd  → Move around
ls  → What's here?

+------------------------+
|    File Ops  📁        |
+------------------------+
mkdir → New folder
touch → New file
cat   → Read file
cp    → Copy
mv    → Move/Rename

+------------------------+
|    Vi Editor ✏️        |
+------------------------+
i     → Insert mode
Esc   → Command mode
:wq!  → Save & exit
:q!   → Exit no save
```

## Tips & Tricks 💡
- Use Tab for auto-completion
- Press ↑ to access previous commands
- Use `clear` to clean terminal screen
- Combine commands with `&&`

Ready to master the terminal? Start practicing these commands! 🚀