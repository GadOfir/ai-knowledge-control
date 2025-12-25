# README.md – System Operational Master

## 🏁 System Onboarding: [░░░░░░░░░░] 0%

> Status: FINAL VALIDATION | Goal: Transition to PRODUCTION.

---

## System Overview (Authority & Scope)

This repository is a **routing-first, capability-controlled Obsidian Knowledge Vault**. It ensures all AI actions are deterministic and safe through strict data typing (**Data, Skill, Project**).

> [!INFO] **Why?**  
> By categorizing knowledge, the AI never guesses which rules to follow. It knows whether it's reading reference facts (Data), step-by-step procedures (Skill), or active work tracking (Project).

---

## Execution Prompt (Runtime Authority)

**You are operating inside a capability-controlled Obsidian Knowledge Vault.**

- **Authority:** `README.md` is the **Single Source of Truth**.  
- **Safety:** The AI is **FORBIDDEN from writing to original files directly**.  
- **Protocol:** All changes (Logs, Notes, Logic) **MUST** be staged in `_update` files and approved by the user before merging.

---

## 1. Global Update Strategy & Authority

**UPDATE_STRATEGY =** `1`

| Value | Behavior |
|-------|---------|
| **1 – Build** | Stage **ALL** data (Notes, Logs, Structure) in `_update` files for user review. |
| **2 – Proposal** | Ask for permission _before_ even creating an `_update` file. |
| **3 – Read-Only** | No writes allowed; validate routing and logic only. |

---

## 2. Master Vault Registry (Index & Paths)

_The AI must maintain this table. Any file/container not listed here is "Invisible" to the system._

| CID  | Name   | Type  | Capability / Purpose            | Authoritative Path |
|------|--------|-------|--------------------------------|------------------|
| R01  | README | Skill | System Authority & Routing      | `README.md`      |

---

## 3. Unified Execution Brain (Routing & Growth)

### Phase A: Routing (Decision Chain)
1. **Consult R01:** Establish global rules and current strategy.  
2. **Locate Context:** Search Section 2 Registry for CIDs whose Purpose/Capability matches the user's request  
3. **Execute:** If found, open that file, read its Execution Prompt, and follow those instructions combined with global rules 

### Phase B: Growth (Pre-Creation Protocol)
If no relevant CID is found, follow this protocol:

1. **Inquiry:** Ask the user for scope and existing knowledge to be captured.  
2. **Missing Info:** Identify missing technical details (ports, hostnames, permissions).  
3. **Registry Proposal:** Propose a new CID, Type, and Path for Section 2.

---

## 4. Shadow Staging & Reconciliation (Strict Safety)

- **Staging:** Create `filename_update.md` for **ANY change to vault content.**
- **No Direct Writing:** The AI will never modify an original file without a staged proposal.  
- **Reconciliation:** Compare `_update` with original → Propose to user → Apply only after approval.  
- **Cleanup:** Delete `_update` files immediately after successful reconciliation.
- **Manual Changes:** If user manually modifies a file, create `filename_update_afterAIreview.md` to review and reconcile changes.

---

## 5. Vault Expansion & Autonomy Policy

- **Data & Skill Files:** Requires individual user confirmation and Registry entry for every file.  
- **Project Autonomy:** Requires confirmation for the **Project Root Folder** and **Index File** only.  
- **Local Freedom:** Inside an approved Project Folder, the AI may create sub-folders and files (logs, artifacts) without individual Registry entries, provided they are linked in the Project Index.
- **Folder Rules:** Root has only README.md; project files/data types are created in folders named after the project. Inside Project Folder: AI can create files/subfolders locally. Outside Project Folder: creation forbidden unless allowed by UPDATE_STRATEGY. Always confirm folder scope before acting.

---

## 6. Maintenance & Self-Healing

- **Summarization:** Every 20 entries → propose summary via `_update`.  
- **Self-Healing:** On every 10th operation, verify that all Registry CIDs match actual file metadata. If mismatch found, propose correction via _update.  
- **Path Repair:** If a file is moved, use the CID to find it and update Section 2.

---

## 7. Vault File Template (V1.3)

# <Name> – Vault File (AUTO-GENERATED)

Metadata: [Type: Data | Skill | Project | Strategy: `<UPDATE_STRATEGY>`]  
Active Context: [CID: `<Registry ID>` | Task: `<Current Operation Description>`]
RULE: Use <OPTIONAL_INPUT> for undecided fields or leave blank. Add <!--AI_NOTE--> only when information is solid and not speculative.

### Execution Prompt (Copy & Use)

- Authority: README.md | Update Strategy: Inherited  
- Rules: **STAGING ONLY**. Do not write to original files.  
- Task: `<DESCRIBE GOAL>`  
- Expected Output: A staged `_update` file containing actions/logs for user review.

### Purpose
What this file exists to accomplish.

### Decision Chains  
If-then logic for common scenarios in this domain.

### Common Commands
Frequently used commands/code snippets for this context.

### Common Issues
Known problems and their solutions.

### Key Learnings
Important discoveries from real use.

### Notes
Miscellaneous observations and context.

### Project File Registry (For Project Type Only)

_If Type is Project, maintain this table to track all files in the project. Similar to Master Vault Registry but project-scoped. This IS the "Project Index" referenced in Section 5._

| File Path | Purpose | Created By |
|-----------|----------|-------------|
| `<relative/path/to/file.md>` | `<Why this file exists>` | `User Request` or `AI Initiative` |

---

## 8. [SYSTEM STATE: INITIALIZING]

- **Next Step:** Confirm onboarding → promote to Production.
- **No active projects registered**
- **No skill files registered**
- **Vault ready to begin setup**

---

### End of README
