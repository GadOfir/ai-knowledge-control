1. i want to simplefy my MD file

2. some parts are getting to overloaded i want to reduce the data slop

3. improve the part about working with any folder not just obsidean, we just need mcp that can write to files 

4. simplfy onboading life cycle
5. 



# README.md - System Operational Master V1.2 - ^ ok 

## System Onboarding: [----------] 0% - ^ simplfy

---

## System Overview (What This System Is)

This repository is a **routing-first, capability-controlled Obsidian Knowledge Vault**. It ensures all AI actions are deterministic and safe through strict data typing (**Data, Skill, Project**). ^i want to change this so not only obsidean but it can use obsidean for conviance , any MCP with abilty to write to files


> [!INFO] **Why?**  
> By categorizing knowledge, the AI never guesses which rules to follow. It knows whether it's reading reference facts (Data), step-by-step procedures (Skill), or active work tracking (Project). ^ - micro steamnt check if needed or just for humen info

---

## Execution Prompt (Runtime Authority) ^ make sure it will get auto repaierd each time we optmzie ceack how much it will take us to optmize each run and is it worth it

**You are operating inside a capability-controlled Obsidian Knowledge Vault.**

- **Authority:** `README.md` is the **Single Source of Truth**
- **System Status:** TEMPLATE (awaiting onboarding)
- **Update Strategy:** 1 (Build/Stage mode)
- **Safety:** The AI is **FORBIDDEN from writing to original files directly**
- **Protocol:** All changes (Logs, Notes, Logic) **MUST** be staged in `_update` files and approved by the user before merging

---

## 1. Global Update Strategy & Authority (Write Permission Modes)

**UPDATE_STRATEGY =** `1` ^ make sure it will get auto repaierd each time we optmzie ceack how much it will take us to optmize each run and is it worth it

|Value|Behavior|
|---|---|
|**1 - Build**|Stage **ALL** data (Notes, Logs, Structure) in `_update` files for user review.| ^ we need less data in temaplte and make the promt auto corect each time we update the reamde 2
|**2 - Proposal**|Ask for permission _before_ even creating an `_update` file.| ^ want to remove this 
|**3 - Read-Only**|No writes allowed; validate routing and logic only.| ^ ok but lets think cerffuly abot this again how do incoparete this better now that 2 is gonw When to Use Each Strategy:


 
**When to Use Each Strategy:**
- **Strategy 1 (Build/Stage):** Development and validation phases - active feature work ^ we need less data in temaplte and make the promt auto corect each time we update the reamde
- **Strategy 2 (Proposal):** Conservative development - sensitive operations requiring extra caution - ^ want to remove this 
- **Strategy 3 (Read-Only):** Production vaults - immutable references, no modifications allowed ^ ok but lets think cerffuly abot this again how do incoparete this better now that 2 is gonw When to Use Each Strategy:

**Current Configuration:**
- UPDATE_STRATEGY = 1 (Build/Stage mode) ^ ok
- SYSTEM_STATUS = TEMPLATE (see Section 8) ^ lets see how we imrpvoe onboadring we want to simplfy it
- This combination is appropriate for a fresh vault awaiting onboarding

---

## 2. Master Vault Registry (Index & Paths)  ^ this is the best part of the system we want to give this part the best attenation


_The AI must maintain this table. Any file/container not listed here is "Invisible" to the system._

| CID | Name   | Type  | Capability / Purpose       | Authoritative Path |
| --- | ------ | ----- | -------------------------- | ------------------ |
| R01 | README | Skill | System Authority & Routing | `README.md`        |

**Maintenance Protocol:**
- All Registry updates **MUST** be staged in `README_update.md`
- Never edit Registry directly (violates UPDATE_STRATEGY)
- Add entries during Phase B (Growth) via staging mechanism
- Self-Healing (Section 6) validates registry every 10 operations
- User approves all registry changes before merging

---

## 3. Unified Execution Brain (Routing & Growth)

### Phase A: Routing (Decision Chain)

1. **Consult R01:** Establish global rules and current strategy.
2. **Locate Context:** Search Section 2 Registry for CIDs whose Purpose/Capability matches the user's request
3. **Validate CID Structure:**
   - Skill/Project CIDs: Must have Execution Prompt section
   - Data CIDs: Must have Authority declaration
   - If malformed: Report error to user, suggest fixing CID or removing from Registry
4. **Execute:** If valid, open that file, read its Execution Prompt, and follow those instructions combined with global rules

### Phase B: Growth (Pre-Creation Protocol)

If no relevant CID is found, follow this protocol:

1. **Inquiry:** Ask the user for scope and existing knowledge to be captured.
2. **Missing Info:** Identify missing technical details (ports, hostnames, permissions).
3. **Registry Proposal:** Propose a new CID, Type, and Path for Section 2.

---

## 4. Shadow Staging & Reconciliation (Strict Safety)

- **Staging:** Create `filename_update.md` for **ANY change to vault content.** - ^unelss i ask you
- **No Direct Writing:** The AI will never modify an original file without a staged proposal.
- **Reconciliation:** Compare `_update` with original → Propose to user → Apply only after approval. ^ update execation promt and optmzie file for slop
- **Cleanup:** Delete `_update` files immediately after successful reconciliation.

---
 
## 5. Vault Expansion & Autonomy Policy (Growth Control Rules) ^the skiils dont go to the project folder this genral to the agent

- **Data & Skill Files:** Requires individual user confirmation and Registry entry for every file.
- **Project Autonomy:** Requires confirmation for the **Project Root Folder** and **Index File** only.
- **Local Freedom:** Inside an approved Project Folder, the AI may create sub-folders and files (logs, artifacts) without individual Registry entries, provided they are linked in the Project Index.

**Folder Structure Rules (Enforced):** ^the skiils dont go to the project folder this genral to the agent 
- **Vault root:** Only README.md allowed
- **Data CIDs:** Must be in `/data/` folder
- **Skill CIDs:** Must be in `/skills/` folder
- **Projects:** Must be in `/projects/{{project-name}}/` folder
- **Violation:** AI must refuse and propose correct location

**Folder Scope:**
- Root has only README.md; project files/data types are created in folders named after the project
- Inside Project Folder: AI can create files/subfolders locally (still via staging)
- Outside Project Folder: creation forbidden unless allowed by UPDATE_STRATEGY
- Always confirm folder scope before acting

---

## 6. Maintenance & Self-Healing (Auto-Repair & Cleanup) ^ lets downsize here 
^and just fix the imporntent stuff
^we shuld fix excutain promt each time we update a file 

- **Summarization:** Every 20 new files created → propose summary via `_update`.  
  (Does NOT include `_update` files or temporary files) ^ get rid of that 

- **Self-Healing:** On every 10th operation, verify that all Registry CIDs match actual file metadata. If mismatch found, propose correction via `_update`.^ get rid of that 

- **Registry Validation:** Every 10 operations, verify: ^ get rid of that 
  - All Registry paths point to existing files
  - All CID files have required sections (Execution Prompt or Authority)
  - Propose cleanup for broken/malformed CIDs via `_update`

- **Path Repair Process:**
  1. Detect: Registry CID points to non-existent file
  2. Search: Scan vault for files with matching CID in metadata header
  3. Propose: Stage Registry update in `README_update.md`
  4. Verify: User confirms new path is correct
  5. Update: Merge registry change after approval

---

## 7. Vault File Template V1.4 (Standard File Structure)

### For Skill/Project/Data CIDs (Type: Skill | Project | Data) ^ add data type to this temaplte also but dont use the same temaple values 
make a rule in it

```markdown
# Vault File (AUTO-GENERATED)

Metadata: [Type: Skill | Project | Strategy: {{UPDATE_STRATEGY}}]  
Active Context: [CID: {{Registry ID}} | Task: {{Current Operation Description}}]

RULE: Use {{OPTIONAL_INPUT}} for undecided fields or leave blank. Add only when information is solid and not speculative.

## Execution Prompt (Copy & Use)

- Authority: README.md | Update Strategy: Inherited
- Rules: **STAGING ONLY**. Do not write to original files.
- Task: {{DESCRIBE GOAL}}
- Expected Output: A staged `_update` file containing actions/logs for user review.

## Purpose

What this file exists to accomplish.

## Decision Chains




## Key Learnings ,Common Issues , Common Commands, Notes




## Project File Registry (For Project Type Only)

_If Type is Project, maintain this table to track all files in the project. Similar to Master Vault Registry but project-scoped. This IS the "Project Index" referenced in Section 5._

|File Path|Purpose|Created By|
|---|---|---|
|{{relative/path/to/file.md}}|{{Why this file exists}}|User Request or AI Initiative|
```

---

### For Data CIDs (Type: Data)
^ (combine the two temapltes , and make rules , this is too long for the tempalte , make it smarter )
```

---

## 8. System Status & Lifecycle - simply the entire on borading an lifexcycle 

**SYSTEM_STATUS =** `TEMPLATE`  
**Version:** v1.2-CANDIDATE  
**Update Strategy:** 1 (Build/Stage)

### Lifecycle States

| State | Description | When | UPDATE_STRATEGY |
|-------|-------------|------|-----------------|
| **TEMPLATE** | Fresh vault, ready for onboarding | Before any CIDs created | 1 (Build/Stage) |
| **ACTIVE** | Operational vault in use | After onboarding, CIDs exist | 1 (Build/Stage) |

**Current Phase:** TEMPLATE - Awaiting onboarding and first CID creation

**Transition:**
- **TEMPLATE → ACTIVE:** When first Data/Skill/Project CID is created
- **Status Change:** User-initiated (manual update to this section)

**Active Resources:**
- **Projects:** 0 (ready for creation)
- **Skills:** 0 (ready for creation)
- **Data CIDs:** 0 (ready for creation)
- **Registry Size:** 1 (R01 only - clean template)

**Next Steps:**
1. User onboards by creating first CID (Data/Skill/Project)
2. Update SYSTEM_STATUS to ACTIVE in this section
3. Begin normal operations with CID-based routing

---

### End of README
