# README.md – System Operational Master

## 🏁 System Onboarding: [██░░░░░░░░] 20%

> **Status:** ENVIRONMENT_SYNCED | **Goal:** Initialize Registry & Skills.
> 
> **Expert Shortcut:** Type `INIT_COMPLETE` to move this module to `vault/miscellaneous.md`.

---

### System Overview (Authority & Scope)
This repository is a **routing-first, capability-controlled Obsidian Knowledge Vault**. It ensures all AI actions are deterministic and safe through strict data typing (**Data, Skill, Project**).

> [!INFO] **Why?** > By categorizing knowledge, the AI never guesses which rules to follow; it knows if it's looking at a "How-to" (**Skill**) or a "Working Draft" (**Project**).

### Execution Prompt (Runtime Authority)
You are operating inside a capability-controlled Obsidian Knowledge Vault.
- **Authority:** `README.md` is the **Single Source of Truth**.
- **Safety:** The AI is **FORBIDDEN** from writing to original files directly.
- **Protocol:** All changes (Logs, Notes, Logic) **MUST** be staged in `_update` files and approved by the user before merging.

---

### 1. Global Update Strategy & Authority
**UPDATE_STRATEGY = 1**

| Value | Behavior |
| :--- | :--- |
| **1 – Build** | Stage **ALL** data (Notes, Logs, Structure) in `_update` files for user review. |
| **2 – Proposal** | Ask for permission *before* even creating an `_update` file. |
| **3 – Read-Only** | No writes allowed; validate routing and logic only. |

---

### 2. Master Vault Registry (Index & Paths)
*The AI must maintain this table. Any file/container not listed here is "Invisible" to the system.*

| CID | Name | Type | Capability / Purpose | Authoritative Path |
| :--- | :--- | :--- | :--- | :--- |
| **R01** | README | Logic | System Authority & Routing | `README.md` |

---

### 3. Unified Execution Brain (Routing & Growth)

**Phase A: Routing (Decision Chain)**
1. **Consult R01:** Establish global rules and current strategy.
2. **Locate Context:** Search Section 2 for existing CIDs matching the task.
3. **Execute:** If found, use the approved file's Execution Prompt.

**Phase B: Growth (Pre-Creation Protocol)**
If no relevant CID is found, follow this protocol:
1. **Inquiry:** Ask the user for scope and existing knowledge to be captured.
2. **Missing Info:** Identify missing technical details (ports, hostnames, permissions).
3. **Registry Proposal:** Propose a new CID, Type, and Path for Section 2.

---

### 4. Shadow Staging & Reconciliation (Strict Safety)
- **Staging:** Create `filename_update.md` for **ANY** change (Logic, Logs, or Notes).
- **No Direct Writing:** The AI will never modify an original file without a staged proposal.
- **Reconciliation:** Compare `_update` with original → Propose to user → Apply only after approval.
- **Cleanup:** Delete `_update` files immediately after successful reconciliation.

---

### 5. Vault Expansion & Autonomy Policy
- **Data & Skill Files:** Requires individual user confirmation and Registry entry for every file.
- **Project Autonomy:** Requires confirmation for the **Project Root Folder** and **Index File** only.
- **Local Freedom:** Inside an approved Project Folder, the AI may create sub-folders and files (logs, artifacts) without individual Registry entries, provided they are linked in the Project Index.

---

### 6. Maintenance & Self-Healing
- **Summarization:** Every 20 entries → propose summary via `_update`.
- **Self-Healing:** Periodically verify that all Registry CIDs match file metadata.
- **Path Repair:** If a file is moved, use the CID to find it and update Section 2.

---

### 7. Vault File Template (V1.3)
# <Name> – Vault File (AUTO-GENERATED)
**Metadata:** [Type: Data | Skill | Project | Strategy: <UPDATE_STRATEGY>]
**Active Context:** [ID: <Context ID> | Task: <Description>]

#### Execution Prompt (Copy & Use)
- **Authority:** `README.md` | **Update Strategy:** Inherited
- **Rules:** **STAGING ONLY**. Do not write to original files.
- **Task:** <DESCRIBE GOAL>
- **Expected Output:** A staged `_update` file containing actions/logs for user review.

---

### 9. [SYSTEM STATE: INITIALIZING]
- **Environment:** Platform: `Windows` | Client: `Cursor` | Executor: `PowerShell`
- **Next Step:** Type **`INIT_COMPLETE`** to finalize onboarding or suggest a new Skill/Data file for the Registry.

**End of README**
