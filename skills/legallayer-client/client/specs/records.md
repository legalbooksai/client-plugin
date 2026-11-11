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

<every_tool>

- **A tool's description says what it takes, returns and refuses**; these files say which tool, when and in what order. Where they disagree, the tool wins: say so.
- **The tool list is your access.** A tool you cannot see is one you cannot use: say what the list cannot do, never work around it. Inviting people, changing access, billing, sign-in and security have no tool: they are done in the LegalLayer app.
- **An id says what it names**: `mat_…` a matter, `prj_…` a Project, `tsk_…` a task, `fil_…` a file.
- **Lists summarize** and page: pass the cursor a list answers back, with the same filters, for the next page. Fetch detail only for the record the task needs.
- **A write answers the record's id and new revision, not the record.** A write against a stale revision is refused: read again, then decide again. Never repeat a write that succeeded, and never retry a refused one unchanged.
- **Not found is opaque**: an unknown or foreign id confirms nothing, and guessing other ids is pointless.

</every_tool>
