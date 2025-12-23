README.md – Phase 1.1 (Operational Master)🎯 System OverviewThis repository defines a routing-first, MCP-controlled Obsidian Knowledge Vault. It enables an AI or human operator to:Read structured knowledge.Make deterministic decisions.Execute real actions via MCP servers.Safely grow and optimize the vault over time.[!IMPORTANT]This README.md is the Single Source of Truth for routing, update strategy, and execution authority.🏗️ Core ComponentsClaude Desktop (AI Agent): Primary reasoning and orchestration engine.Obsidian MCP + Vault: Structured, persistent knowledge storage.MCP Shell Runner (desktop-commander): Enables real-world execution under strict routing rules.⚡ Execution Prompt (Copy & Use)Use this prompt when starting a new session or explicitly invoking this vault.MarkdownYou are operating inside an MCP-controlled Obsidian Knowledge Vault.

### Global Rules:
1. You MUST read and follow this README.md before accessing any other file.
2. This file is the Single Source of Truth for logic and execution.
3. `_update` files are staging-only; DO NOT read or execute them during runtime.
4. If required information is missing, STOP and ask the user.

### Update Strategy:
- Follow the defined UPDATE_STRATEGY.
- Creation of new vault files ALWAYS requires explicit user confirmation.

### Task:
<DESCRIBE YOUR GOAL HERE>
📋 Prompt Quality ChecklistClarity: States context/scope; uses deterministic language.Safety: References README.md; forbids runtime use of _update files.Completeness: Includes context, constraints, and defined routing.1. Operating ContextAttributeConfiguration ValueLocal Platform`Primary Local Executor``2. Global Update StrategyUPDATE_STRATEGY = 1ValueModeBehavior1Build modeCreate _update for structure; Directly append notes/commands to Vault.2Proposal modeAsk before creating/updating any file or appending notes.3Test modeRead-only; validate routing and logic only.3. Capability Registry (MCP Servers)Name: desktop-commanderPrimary Capabilities: ``Vault Location: ``4. Canonical Paths RegistryBase Vault Directory: ./vault/Archive Directory: ./vault/archive/Authoritative PathDescriptionREADME.mdRoot ContextFrequently Used Paths:(Add as discovered and approved)5. Task Classification & Decision ChainsStructure: Decision Chain → Context Source → Primary Knowledge → Fallback → ExecutionConsult README.mdLocate existing Vault contextExecute using the appropriate MCP6. Shadow Update Mechanism (_update)Purpose: Stage structural changes safely.Required for: Logic updates, refactors, and structural changes.Must explain: Observed state, reason for change, and affected section.7. Optimization & Reconciliation PolicyCompare _update with original.Propose changes; apply only after approval.Update readme_update.md if global behavior changes.8. Vault Creation & Expansion PolicyTriggers: New MCP servers or Major Epics/Skills.Mandatory: Sections 3 and 4 MUST be updated upon file creation.Logs: Assign Context IDs to all command logs.Approval: User confirmation required for every new file.9. Maintenance & Self-OptimizationSummarization: Propose summary via _update every 20 entries.Archiving: No data deletion without moving to ./vault/archive/.10. Pre-Creation Protocol (Inquiry First)Before creating any new vault file, AI MUST ask:Scope: What is the boundary?Knowledge: What existing info should be captured?Missing Info: What technical details are needed?Registry: Confirm Section 3 update.11. Vault File Template (V1.2)Markdown# <Name> – Vault File
**Metadata:** [Logic: Phase 1.1 | Strategy: <UPDATE_STRATEGY>]
**Active Context:** [ID: <Context ID> | Task: <Description>]

## Execution Prompt (Copy & Use)
<INSERT_PROMPT_HERE>

## Purpose
- Describe skill or epic scope.

## Decision Chains
- Local chains for this file.

## Common Commands
- Frequently used commands.

## Common Issues
- Errors (Testing | Infrastructure | Unknown).

## Key Learnings
- Summarized insights.
12. Onboarding & System Start (TEMPORARY)Status: [PENDING INITIALIZATION]Once the first vault file is created:Move onboarding text to vault/miscellaneous.md.Remove this section from README.md.System enters Production Mode.End of README
