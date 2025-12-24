# README.md – Phase 1.1 (Operational Master)

---

## System Overview (Authority & Scope)

This repository defines a **routing-first, data / skill / project–controlled Obsidian Knowledge Vault**.

Its purpose is to allow an AI or human operator to:

- Read structured knowledge
    
- Make deterministic decisions
    
- Execute real actions via skills and projects
    
- Safely grow and optimize the vault over time
    
Start of README
This `README.md` file is the **entry point, authority, and safety boundary** for the entire system.


    
---

## Execution Prompt (Runtime Authority)

Use this prompt when starting a new session or explicitly invoking this vault.

**You are operating inside a capability-controlled Obsidian Knowledge Vault (data / skills / projects)**.

Global Rules:

- You MUST read and follow this `README.md` before accessing any other file.
    
- This file is the **Single Source of Truth** for routing, update strategy, and execution authority.
    
- `_update` files are staging-only and MUST NEVER be read or executed during runtime.
    
- Always follow Decision Chains and strict priority order.
    
- If required information is missing, STOP and ask the user.
    

Update Strategy:

- Follow `UPDATE_STRATEGY` defined below.
    
- Creation of new vault files ALWAYS requires explicit user confirmation.
    

Task:  
`<DESCRIBE YOUR GOAL HERE>`

Constraints:

- Do not assume paths, credentials, or environments.
    
- Prefer existing vault files over creating new ones.
    
- New vault files are only for new data sources, skills, or major projects.
    

Expected Output:

- Clear actions taken or proposed
    
- Correct capability routing (data → skill → project)
    
- No uncontrolled writes
    

---

## Prompt Quality Checklist (Design-Time Only)

All **Execution Prompts** in this repository (README and Vault files) must meet this checklist.

### 1. Clarity

- Explicitly states context and scope
    
- Uses deterministic language
    
- Avoids vague verbs (“handle”, “maybe”, “try”)
    

### 2. Safety

- References README.md as authority
    
- Respects `UPDATE_STRATEGY`
    
- Forbids runtime use of `_update` files
    
- Prevents silent writes or file creation
    
- Instructs to stop and ask when information is missing
    

### 3. Completeness

- Includes context
    
- Defines constraints
    
- Describes expected output
    
- Specifies routing expectations (Decision Chains / capabilities)
    

**Prompt Optimization Rules**

- Prompts may be optimized only via `_update` files
    
- Optimization must state which checklist item is improved and why
    
- Runtime execution always uses the approved prompt in the main file
    

---

## 1. Operating Context (USER MUST FILL)

- **Local Platform:** ``
    
- **AI Client:** ``
    
- **Primary Local Executor (skill / runner):** ``

    ## Conceptual Model (Data / Skills / Projects)


- **Data**  
  Static or dynamic environment details, facts, configuration, or context  
  (e.g. environment details, system state, tenant info)

- **Skill**  
  Instructions that define *how the AI should act*  
  (e.g. testing procedures, analysis rules, behavioral constraints)

- **Project**  
  Goal-oriented work units with scope and intent  
  (e.g. testing project, new development effort, investigation plan)

All routing, decision chains, and execution logic operate on these three types.

---

## 2. Global Update Strategy & Authority

**UPDATE_STRATEGY =** `1`

|Value|Behavior|
|---|---|
|**1 – Build mode**|Create `_update` files for structural changes; directly append small notes/commands to existing vault files|
|**2 – Proposal mode**|Ask before creating or updating any `_update` file or appending notes|
|**3 – Test / read-only mode**|No writes, no `_update` files; validate routing and logic only|

**Authority Rules**

- README.md is the **Single Source of Truth**
    
- All skills and projects must read this file before any execution
    
- Conflicts → README.md wins
    
- `_update` files are never used at runtime
    

---

## 3. Available Data, Skills, and Projects

_(Capability Registry – must have a corresponding vault file)_


- **Name:** 
    
    - **Primary capabilities:**
        
    - **Vault location:**

    - - **Type: Data | Skill | Project:**

---

## 4. Canonical Paths Registry (Authoritative)

**Authoritative Paths**

- `README.md`: Root Context
    

**Frequently Used Paths**

- _(Add as discovered and approved)_
    

---

## 5. Task Classification & Decision Chains
**This section defines how tasks are routed from context to execution.**
**Decision Chain Structure (Strict Priority)**

Decision Chain  
→ Context Source  
→ Primary Knowledge Source  
→ Fallback Source  
→ Skill or Project Execution

Execution Order:

1. Consult README.md
    
2. Locate existing vault context
    
3. Execute using the appropriate skill or project
    

Skip irrelevant chains.  
Always follow priority order.

---

## 6. Shadow Update Files (`_update` Mechanism)

**Purpose:** Stage changes safely without overwriting originals.

Rules:

- Required for structural changes, logic updates, refactors
    
- Governed by `UPDATE_STRATEGY`
    
- Must explain:
    
    - What was observed
        
    - Why change is needed
        
    - What section is affected
        

---

## 7. Optimization & Reconciliation Policy

1. Compare `_update` file with original
    
2. Propose changes to the user
    
3. Apply only after approval
    
4. Update `readme_update.md` if global behavior changes

5. Check if Execution Prompt needs Optimization
    

---

## 8. Vault Creation & Expansion Policy

- New vault files only for:
    
    - New data sources
        
    - New skills
 
    - Major projects
        
- README Sections 3 and 4 MUST be updated upon creation
    
- Cross-link related files
    
- Assign Context IDs to logs
    
- User confirmation required for every new file
    
- Frequently used paths must be proposed for registry inclusion
    

---

## 9. Ongoing Maintenance (Post-Approval Only)

- Every 20 entries → propose summary via `_update`
    
- No data deletion without archiving
    
- Approved insights mirrored into README.md
    

---

## 10. Pre-Creation Protocol (Inquiry First)

Before creating any new vault file, AI MUST ask:

1. What is the scope?
    
2. What existing knowledge should be captured?
    
3. What information is missing?
    
4. Confirm registry update
    

---

## 11. Vault File Template (V1.2)
# <Name> – Vault File (AUTO-GENERATED)
**Metadata:** [Type: Data | Skill | Project | Logic: Phase 1.1 | Strategy: <UPDATE_STRATEGY>]
**Active Context:** [ID: <Context ID> | Task: <Description>]

## Execution Prompt (Copy & Use)

Context:
- Vault File: <Name>
- Authority: README.md
- Update Strategy: Inherited

Rules:
- `_update` files are never used at runtime
- Follow Decision Chain strictly
- Ask before creating new files

Task:
<DESCRIBE WHAT YOU WANT TO DO>

Expected Output:
- Actions taken or proposed
- Commands or issues logged
- Clear next steps

## Purpose
- Describe skill or epic scope

## Decision Chains
- Local chains for this file

## Common Commands
- Frequently used commands

## Common Issues
- Errors (Testing | Infrastructure | Unknown)

## Key Learnings
- Summarized insights

## Notes
- Observations and context references


---

## 12. Onboarding & System Start (TEMPORARY)

**Status:** `[PENDING INITIALIZATION]`

Once the first vault file is created:

- Move onboarding text to `vault/miscellaneous.md`
    
- Remove this section from README.md
    
- System enters Production Mode
    

---

### End of README
