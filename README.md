

# 📘 TIA Portal & Git Integration via VCI Connector

## Overview

This guide explains how to use **VCI Connector** to integrate **TIA Portal** with **GitHub**, enabling version control of:

- Functions  
- Function Blocks  
- UDTs  
- Faceplates  
- Documentation (e.g., via Code2Docu)

Changes are tracked in Git and can be shared across machines.

---

## 🛠 Requirements

- TIA Portal V16+
- VCI Connector
- Git (CLI or GUI)
- GitHub repository
- Optional: Code2Docu for auto-generated docs or Print to PDF from TIA Portal

---

## 🔧 Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/your-tia-project.git
```

### 2. Configure VCI Connector

- Set project root to the cloned repo
- Enable TIA Portal integration
- Track:
  - `.ap14` / `.ap16` files
  - XML exports of blocks
  - `/docs` folder for documentation

### 3. Open in TIA Portal

- Open the project from the Git-tracked folder
- Edit blocks, UDTs, faceplates, and documentation

### 4. Save & Commit

```bash
git add .
git commit -m "Updated motor control logic"
git push origin main
```

### 5. Sync on Other Machines

```bash
git pull origin main
```

Open the updated project in TIA Portal.

---

## 📄 Documentation (Optional)



- Generate docs into `/docs`
- Track with Git for version control

---

## ✅ Tips

- Use branches for features
- Commit regularly with clear messages
- Keep docs synced with code


---

## 🧩 Troubleshooting

- VCI not syncing → Check repo path
- TIA Portal crashes → Ensure project isn’t locked
- Git conflicts → Use `git status` and resolve

---
