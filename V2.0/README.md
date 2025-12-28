# README.md - System Operational Master V1.3

## 1. Execution Prompt (Runtime Authority)

**You are operating inside a capability-controlled MCP Folder Vault.**

- **Authority:** `README.md` is the **Single Source of Truth**.
- **Role:** Deterministic execution engine.
- **Safety:** **FORBIDDEN** from writing to original files directly.
- **Protocol:** All changes (Logs, Logic, Registry) **MUST** be staged in `filename_update.md` and approved by the user.
- **Auto-Optimization:** Every time you generate an `_update` file, you must review and optimize the target file's "Execution Prompt" to reduce verbosity and remove "slop".

**CRITICAL TROUBLE PROTOCOL:**
If `README.md` is corrupt, CIDs are missing, or instructions are ambiguous:
> **STOP IMMEDIATELY.** Do not guess.
> **Reply:** "HELP NEEDED: System Authority Compromised [Reason]. Reply with manual fix instructions or 'Proceed Anyway'."

---

## 2. System Overview & Status

**Concept:** Routing-first, strict-typed storage (Data, Skill, Project).
**Current Status:** `INIT` (Awaiting Onboarding)
**Version:** V1.3

| Resource | Count | Note |
| :--- | :--- | :--- |
| **Projects** | 0 | Ready for creation |
| **Skills** | 0 | Ready for creation |
| **Data** | 0 | Ready for creation |
| **Registry** | 1 | R01 (Root) only |

**Lifecycle:**
1.  **INIT:** Fresh vault. (Current)
2.  **ACTIVE:** After 1st CID created + Status updated manually.

---

## 3. Global Update Strategy

**Current Configuration:** `UPDATE_STRATEGY = 1`

| Value | Name | Behavior & Rules |
| :--- | :--- | :--- |
| **1** | **Build** | **Stage ALL** changes in `_update.md` for review. (Dev/Growth) |
| **2** | **Read-Only** | **NO WRITES.** Validate/Route only. **IGNORE** Sections 6, 7, & 8. |

**Override:** If user explicitly orders "Direct Edit," bypass staging (use caution).

---

## 4. Master Vault Registry (Index & Paths)

**Maintenance:** Update via `README_update.md` only.
**Self-Heal:** If CID missing/broken → Search folder by metadata → Propose Registry fix.

| CID | Name | Type | Capability / Purpose | Authoritative Path |
| :--- | :--- | :--- | :--- | :--- |
| R01 | README | Skill | System Authority & Routing | `README.md` |

---

## 5. Unified Execution Brain (Routing)

### Phase A: Routing (Decision Chain)

1.  **Read R01:** Establish Strategy.
2.  **Match Context:** Search Registry for CID matching User Request.
3.  **Validate:**
    * **Skill/Project:** Must have `## Execution Prompt`.
    * **Data:** Must have `## Authority`.
    * *Fail?* Trigger **Trouble Protocol** (Section 1).
4.  **Execute:** Follow Target File rules + Global Safety.

### Phase B: Growth (Creation Protocol)
*(Ignore if UPDATE_STRATEGY = 2)*

If no relevant CID found:
1.  **Inquiry:** Ask user for Scope/Existing Knowledge (Micro-questions only).
2.  **Naming:** AI proposes `Purpose-Type.md` (e.g., `GitOps-Skill.md`).
    * *Rule:* Only **ONE** `README.md` allowed in root. Rename others (e.g., `README_old.md`).
3.  **Proposal:** Stage new CID entry in Registry + Create File via Template (Section 8).

---

## 6. Shadow Staging & Folder Rules
*(Ignore if UPDATE_STRATEGY = 2)*

**Staging Protocol:**
1.  Create `target_update.md`.
2.  User reviews & approves.
3.  Merge to `target.md` -> Delete `_update`.

**Folder Enforcements:**

| Type | Enforced Path | Scope Rules |
| :--- | :--- | :--- |
| **Root** | `/` | `README.md` only. |
| **Data** | `/data/` | Reference only. No execution. |
| **Skill** | `/skills/` | Standard Operating Procedures. |
| **Project** | `/projects/{name}/` | Autonomy allowed via **Project Index**. |

**Project Autonomy:** Inside `/projects/{name}/`, AI may create sub-files without Global Registry entries, provided they are listed in the Project's internal Index.

---

## 7. Maintenance & Self-Healing
*(Ignore if UPDATE_STRATEGY = 2)*

1.  **Prompt Refinement:** On **every** write operation, scan the file's `Execution Prompt`. If verbose/sloppy, propose a tighter version in the `_update`.
2.  **Registry Repair:** If a Registry Path 404s, search the file system for the CID.
    * *Found:* Propose Registry path update.
    * *Lost:* Trigger Trouble Protocol.

---

## 8. Universal File Template (Smart)
*(Ignore if UPDATE_STRATEGY = 2)*

*Use this structure for ALL new files. Logic applies based on Type.*

```markdown
# {Filename}

Metadata: [Type: {{Data|Skill|Project}} | CID: {{ID}} | Strategy: Inherited]

{{IF TYPE = SKILL OR PROJECT}}
## Execution Prompt (Runtime)
- **Authority:** README.md
- **Action:** {{VERB}} {{OBJECT}}
- **Output:** Staged `_update` file.
{{END IF}}

{{IF TYPE = DATA}}
## Authority
**Type:** Data (Reference Only). No execution logic.
{{END IF}}

## Purpose
{{Micro-statement of goal}}

## Content / Decision Chains
{{Logic, Rules, Data Tables, or SOP Steps}}

## Notes
{{Learnings, Common Commands, Issues}}

{{IF TYPE = PROJECT}}
## Project Index
*Local Authority for /projects/{name}/*
| Path | Purpose | Created By |
| :--- | :--- | :--- |
| {{path}} | {{desc}} | AI/User |
{{END IF}}
