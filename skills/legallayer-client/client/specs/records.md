<module>specs/records.md</module>
<title>The records and how every tool behaves</title>

<records>

| Record | What it is |
| --- | --- |
| organization | your company's account with its legal team. Its name is a label and never identifies a legal party. |
| entity | one of your company's legal persons: legal identity only. |
| matter | one legal request: its type, the details asked for, a status, optionally one entity. |
| project | a larger piece of work with a status and a tree of tasks. |
| task | one step of a Project, with its own status. |
| message | one entry in the conversation of a matter, a Project or a task. |
| file | a stored document with versions, of your company and optionally of a matter, a Project, a task or an entity. |
| type | a kind of request or Project your legal team offers, with the details it asks for. |

A **work item** is a matter, a Project or a task.

</records>

<words>

- **A request** is a matter.
- **A deal** is a Project. Say "deal" to the person; the tools, ids and fields say project.
- **An LOI** is the record the tools name a deal (`dea_…`): the terms of a letter of intent settled between two companies. "Deal" means it only when the person gives its id or says LOI. You can read one; agreeing or changing its terms is done by a person in the LegalLayer app.

</words>

<statuses>

One status vocabulary for matters, Projects and tasks, five values: not started, in progress, waiting (stuck on someone's action), completed, canceled. Who a waiting item waits on is read from its conversation, not from the status.

</statuses>

<every_tool>

- **`get_me` first**: who you act as and the organizations your access covers. When it covers more than one and the task does not say which, ask once, then name that organization on every call.
- **The tool list is your access.** A tool you cannot see is one you cannot use: say what the list cannot do, never work around it. Inviting people, changing access, billing, sign-in and security have no tool: they are done in the LegalLayer app.
- **An id says what it names**: `mat_…` a matter, `prj_…` a Project, `tsk_…` a task, `fil_…` a file.
- **Lists summarize** and page: pass the cursor a list answers back, with the same filters, for the next page. Fetch detail only for the record the task needs.
- **A write answers the record's id and new revision, not the record.** A write against a stale revision is refused: read again, then decide again. Never repeat a write that succeeded, and never retry a refused one unchanged.
- **Not found is opaque**: an unknown or foreign id confirms nothing, and guessing other ids is pointless.

</every_tool>
