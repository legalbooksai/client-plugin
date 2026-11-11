<module>specs/files.md</module>
<title>Documents</title>

<finding_and_reading>

- **Finding**: `list_files` for your company, a work item or an entity; its search covers names and stored text. No match is not proof: a file whose text could not be read matches by name only.
- **Reading**: `get_file` lists a file's versions, newest first, and gives a version's text or a download link.

</finding_and_reading>

<uploading>

In this order (`client/specs/rules.md` — rule 3):

1. `create_upload` reserves a short-lived ticket for one file; it creates nothing.
2. Send the file's bytes to the ticket's upload address with every header it gives, before it expires. A ticket takes bytes once: a changed file or a failed upload needs a fresh ticket.
3. Record it: `create_file` for a new document, on the work item it belongs to or among your company's or an entity's own files; `create_file_version` for a newer version of a document already there.

Nothing is deleted: `update_file` renames or re-files a document.

</uploading>
