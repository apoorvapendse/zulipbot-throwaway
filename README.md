# zulipbot-throwaway

Public sandbox for a local copy of [zulipbot](https://github.com/apoorvapendse/zulipbot).

The local process uses Zulip's production example config (`config/config-example.ts` in that repository). The only change is the repository allowlist. This repository is the only one the process is allowed to read or write. It does not operate on `zulip/zulip`.

Commands are addressed to whichever GitHub account the process authenticates as. The bot ignores comments from that same account, so claim and label commands have to come from a different GitHub user.

Area-label comments mention `@apoorvapendse/<team>` using the team slugs from the production config. Those teams are not created on this account. The mention is the same string production would post, with this repository's owner in place of `zulip`.

Labels named by that config are created on this repository, including the size labels, `help wanted`, `in progress`, `has conflicts`, and the area labels from the example map.
