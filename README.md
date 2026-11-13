# LegalLayer

Work with your legal team from Claude. This plugin brings the LegalLayer connector and the skill
that teaches Claude to use it: check on your company's Matters and Projects, ask your legal team
for work, read and answer their messages, find and upload documents.

You need a LegalLayer account. Claude acts as you, with your access and nothing more. Nothing here
is legal advice.

## Install in Claude Code

1. Type `/plugin`, open **Marketplaces**, choose **Add marketplace** and enter `legallayer/client-plugin`.
2. Open **Discover**, select **legallayer-client** and choose **Install**.
3. Restart Claude Code.
4. Type `/mcp`, select **legallayer** and sign in with your LegalLayer account.

From a terminal:

```
claude plugin marketplace add legallayer/client-plugin
claude plugin install legallayer-client@legallayer-client
```

## Other hosts

- **Claude on the web or desktop**: add the connector `https://api.legalbooks.ai/mcp` under
  Settings > Connectors, then add the folder `skills/legallayer-client` as a skill.
- **OpenAI Codex**: `.codex-plugin/plugin.json` names the same `skills/` folder. Not yet tested
  there; add the connector by hand.

## About this repository

It is published from LegalLayer's own source at the commit `SOURCE` names; changes are made
there, not here. Licensed under Apache-2.0 (`LICENSE`).
