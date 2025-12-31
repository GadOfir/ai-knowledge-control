# VAULT CONTROL README

AI acts only when I type:
notes: {VERB} {OBJECT}
notes: check {OBJECT}

VERBS:
add, update, fix, configure, document, review, plan, check

RULES:
- Touch only the file for {OBJECT}
- If exists → update. If missing → create.
- Filename: {OBJECT}.md
- No scanning the whole vault
- Ask once if unclear

FORMAT:
# {OBJECT}
Action: {VERB} {OBJECT}
Log:
- YYYY-MM-DD {entry}

EXAMPLES:
notes: update pfsense
notes: fix sink
notes: configure vpn
notes: check pfsense
