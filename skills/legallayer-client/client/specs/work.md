<module>specs/work.md</module>
<title>Matters, Projects, Terms and messages</title>

<words>

- **A Matter** is one legal request; **a Project** is a larger piece of work, with a tree of tasks (for a deal, a task for each counterparty, and one under it for each document). Answer in the person's own word: their request is a request and their deal a deal to them; the tools, ids and fields say matter and project.
- **Terms** is where two companies negotiate the terms of a term sheet or letter of intent; the tools name its record a deal (`list_deals`, `get_deal`, `dea_…`). The person means Terms only when they name it, give its id or ask about terms being negotiated there; a deal they name is a Project, and an LOI or term sheet they want drafted or reviewed is a request. You can read Terms; agreeing or changing terms is done by a person in the LegalLayer app.

</words>

<statuses>

One status vocabulary for Matters, Projects and tasks, five values: not started, in progress, waiting (stuck on someone's action), completed, canceled. Who a waiting item waits on is read from its conversation, not from the status.

</statuses>

<following>

- **What is open**: `list_matters` and `list_projects`, narrowed by status; `list_tasks` for the tasks of a Project. `get_matter`, `get_project` and `get_task` give one item in full.
- **Where a Project stands**: `get_project` with its tasks shows each task's status and what it waits on.
- **What was said**: `list_messages` by the item reads its whole conversation, newest first. Read it before answering a question about the item (`<statuses>`).
- **Pins** (`add_pin`, `remove_pin`) mark the items the person follows; a list filtered to pinned shows them.

</following>

<asking_for_work>

1. Look for an open item about the same thing first; a second request for the same work splits its conversation.
2. Find the type: the catalog tools list the kinds of request your legal team offers and the details each asks for.
3. Gather those details from the person. Leave out what they do not know (`client/specs/rules.md` — rule 5), and name the entity (`client/specs/rules.md` — rule 2).
4. `create_matter`, once, after the person confirms. It starts not started, with nobody assigned; the legal team takes it from there.

A status, an assignee and the plan of a Project are the legal team's to set. To change or stop a request, say so in its conversation.

</asking_for_work>

<messages>

`create_message` posts in an item's conversation (`client/specs/rules.md` — rule 3). Answer the legal team's question in the conversation it was asked in; start nothing new for it.

</messages>
