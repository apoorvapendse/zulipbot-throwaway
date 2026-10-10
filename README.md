# zulipbot-throwaway

Public sandbox for a local copy of [zulipbot](https://github.com/apoorvapendse/zulipbot).

The local process loads `config/config-example.ts` unchanged. `config/config.ts` is a symlink to that file, which is how the zulipbot CI job loads it. The allowlist in that file is `zulip/zulip`, `zulip/python-zulip-api`, `zulip/zulip-desktop`, `zulip/zulip-terminal`, and `zulip/zulipbot`.

This repository carries the labels that file names, including the size labels, `help wanted`, `in progress`, `has conflicts`, and the area labels. A webhook delivers its events to the local process. The process handles an event only when the repository is on that allowlist.
