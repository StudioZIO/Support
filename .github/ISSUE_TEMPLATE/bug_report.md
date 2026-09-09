---
name: Bug report
about: Something behaves incorrectly, crashes, or does not appear in your host
labels: bug
---

Fill in what you can. The first five lines are what make a report actionable on the first pass rather than the third — the rest is a bonus.

**Plug-in:** Mastering Suite / Tempo Delay

**Plug-in version:** (shown in the plug-in's own status bar, e.g. 2.1.1)

**Format:** AU / VST3 / Standalone

**Host and version:** (e.g. Logic Pro 11.2, Reaper 7.29, Live 12.1)

**macOS version and Mac model:** (e.g. macOS 15.4 on an M2 Pro — Apple Silicon or Intel matters, Tempo Delay has no Intel build)

### What happened

What you did, and what happened instead of what you expected. The smallest sequence that reproduces it is worth more than a long description.

### Screenshots, recording or crash report

Optional. If it crashed, the macOS crash report from Console.app is the fastest route to a fix.

Before posting logs, screenshots, or crash reports, please review them for sensitive information such as personal usernames, local file paths, confidential project names, or client data.

---

Only if the plug-in does not appear in your host — delete this section otherwise:

- [ ] I ran `auval -a | grep -i studiozio` in Terminal, and the result was:
- [ ] I cleared the AU cache with `killall -9 AudioComponentRegistrar` and relaunched the host
- [ ] I confirmed my Mac's architecture matches the build
