<folder>client/</folder>

<description>

How a client's person uses LegalLayer through its MCP tools: which record holds what, which tool when and in what order, and what never to do. LegalLayer is where a company and the legal team serving it work together: the company's requests and deals, their conversations and documents. Its records are authoritative: a current fact comes from them, not from memory.

Nothing here is legal advice, and nothing here replaces the legal team.

</description>

<connector>

The connector is LegalLayer's MCP server, `https://api.legalbooks.ai/mcp` (streamable HTTP). Sign in with your LegalLayer account. The server lists the tools your access admits.

</connector>

<reading>

- **`client/meta.md`** is this overview; **`client/specs/`** holds the detail, one file per topic, read when `<load_next>` or the task calls for it.
- **XML tags** mark a file's sections. A citation names the file and, after a dash, the section or rule in it: `client/specs/rules.md` — rule 2.
- **A fact is stated once** and cited elsewhere. Follow a citation; never fill it in from memory.
- **A tool's description says what it takes, returns and refuses**; these files say which tool, when and in what order. Where they disagree, the tool wins: say so.

</reading>

<load_next>

- `client/specs/records.md` — the records, the words people use for them, statuses, how every tool behaves. Read before any task.
- `client/specs/rules.md` — the rules you keep. Read before any task.
- `client/specs/work.md` — following your requests and deals, asking for legal work, messages.
- `client/specs/files.md` — finding, reading and uploading documents.

</load_next>

<contents>

- `SKILL.md` — the entry: when the skill applies, who you act for, the read order
- `client/meta.md` — this index: `<connector>`, `<reading>`
- `client/specs/` — the detail, one file per topic, as `<load_next>` lists them

</contents>
