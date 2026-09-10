# StudioZIO Support

Bug reports and questions for StudioZIO plug-ins. Open an issue here and it reaches the person who wrote the code.

There is no support ticket system, no account and no queue position. This is the whole thing.

## Products

| Plug-in | Version | System | Site |
| --- | --- | --- | --- |
| StudioZIO Mastering Suite | 2.1.1 | macOS 11+, Universal (Apple Silicon + Intel) | https://studioziomasteringsuite.vercel.app |
| StudioZIO Tempo Delay | 4.0.1 | macOS 12+, Apple Silicon only | https://www.tempodelay.tech |

Downloads and checksums: https://github.com/StudioZIO/StudioZIO-Releases

## Reporting a bug

Open an issue. What makes a report useful, roughly in order:

1. **Which plug-in and version.** The version is in the plug-in's own status bar.
2. **Host and version.** Logic 11.2, Reaper 7.x, Live 12.1, and so on.
3. **macOS version and Mac model.** Tempo Delay is Apple Silicon only.
4. **Plug-in format.** AU, VST3, AAX or Standalone. Several problems only appear in one of them.
5. **What you did, and what happened instead.** The smallest sequence that reproduces it is worth more than a long description.

Screenshots help. A short screen recording helps more. If it crashed, the macOS crash report from Console.app is the fastest route to a fix.

## Before reporting "it doesn't show up"

Most first-run problems on macOS are the same three things:

- **Run `auval` for AU.** In Terminal: `auval -a | grep -i studiozio`. If the plug-in is not listed, the host is not the problem.
- **Clear the AU cache.** `killall -9 AudioComponentRegistrar`, then relaunch the host. A stale entry from an earlier version can persist.
- **Check the architecture.** Tempo Delay is Apple Silicon only. On an Intel Mac it will not appear, and there is no error message anywhere saying so.

If those three do not explain it, please open an issue — that is a real bug in the installer and worth knowing about.

## Feature requests

Welcome, in the same place. It helps to say what you were trying to do rather than which control you want added; the underlying problem is often solvable in a way the request did not anticipate.

## Independent use feedback

If you have used a plug-in in a first session or a real project, the [independent use feedback template](https://github.com/StudioZIO/Support/issues/new?template=independent-use-feedback.md) is the right place for a neutral report. Favourable coverage is not requested or required; mixed and negative findings are useful too. Any permission to quote or link a report is optional.

## Known limits

Stated up front rather than discovered later:

- macOS only. There is no build for any other operating system and none is planned.
- Tempo Delay is Apple Silicon only.

## How issues are handled

### Questions

Questions are answered or clarified, then normally closed once resolved.

### Feature requests

Requests are reviewed for the underlying workflow and product fit. They may remain open temporarily while being considered, but they are not maintained as an indefinite public backlog and do not imply implementation, priority, or delivery dates.

### Bug reports

Reports are investigated and reproduced where possible. A confirmed report does not automatically become a public Known Issues entry. Meaningful defects affecting a current release may be added manually to the StudioZIO Community Known Issues page.

### Independent use feedback

Credible compatibility reports may be reflected manually as `Community Reported`. This does not mean StudioZIO has independently verified the host or system combination. `StudioZIO Verified` is reserved for internal testing.

## Response

One person maintains these. Reports get read. Crashes and anything that produces wrong audio come first; cosmetic issues are fixed when the next release is being prepared either way.

Email, if you would rather not open an issue: studiozioplugins@gmail.com
