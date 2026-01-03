VAULT CONTROL README
Trigger format: notes: {VERB} {OBJECT} notes: check {OBJECT}

VERBS: add, update, fix, configure, document, review, plan

RULES:

File = {OBJECT}.md
If file exists → update; else → create
Log entries: one line only
Do not scan vault
If unsure → ask once
NOTE FORMAT:

{OBJECT}
Action: {VERB} {OBJECT} Log:

YYYY-MM-DD {entry}
EXAMPLES: notes: update pfsense notes: fix sink notes: configure vpn notes: check pfsense
