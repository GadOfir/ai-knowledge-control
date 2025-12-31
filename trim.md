# VAULT CONTROL README

AI acts only when I type:
notes: {VERB} {OBJECT}
notes: check {OBJECT}

VERBS (allowed):
add, update, fix, install, document, review, plan, check

FILE RULES:
- File name = {OBJECT}.md
- If file exists → update it
- If not → create it
- Keep log short

NOTE FORMAT:
# {OBJECT}
Action: {VERB} {OBJECT}
Log:
- YYYY-MM-DD {entry}

EXAMPLES:
notes: update pfsense vpn
notes: fix leaking sink
notes: document family schedule
notes: check pfsense
notes: check plumbing
