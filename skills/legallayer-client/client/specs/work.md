<module>specs/work.md</module>
<title>Requests, deals and messages</title>

<following>

- **What is open**: `list_matters` and `list_projects`, narrowed by status; `list_tasks` for the steps of a deal. `get_matter`, `get_project` and `get_task` give one item in full.
- **Where a deal stands**: `get_project` with its tasks shows each step's status and what it waits on.
- **What was said**: `list_messages` by the item reads its whole conversation, newest first. Read it before answering a question about the item (`client/specs/records.md` — `<statuses>`).
- **Pins** (`add_pin`, `remove_pin`) mark the items the person follows; a list filtered to pinned shows them.

</following>

<asking_for_work>

1. Look for an open item about the same thing first; a second request for the same work splits its conversation.
2. Find the type: the catalog tools list the kinds of request your legal team offers and the details each asks for.
3. Gather those details from the person. Leave out what they do not know (`client/specs/rules.md` — rule 5), and name the entity (`client/specs/rules.md` — rule 2).
4. `create_matter`, once, after the person confirms. It starts not started, with nobody assigned; the legal team takes it from there.

A status, an assignee and the plan of a deal are the legal team's to set. To change or stop a request, say so in its conversation.

</asking_for_work>

<messages>

`create_message` posts in an item's conversation (`client/specs/rules.md` — rule 3). Answer the legal team's question in the conversation it was asked in; start nothing new for it.

</messages>
