I mostly build things I want to use, so there are no half-baked proofs of concept here: every repository contains something I shared only after using it myself.

## Books built with Claude Code

I wanted a long, up-to-date read on each of these subjects, could not find one, so I had to build it.

- [weekend-diy-book](https://github.com/vkorost/weekend-diy-book) (Claude Code: The Definitive Guide): a technical book on agentic development with Claude Code, written by Claude Code. Includes the assignment file that produced it, so you can generate your own.
- [claude-certified-architect-guide](https://github.com/vkorost/claude-certified-architect-guide): a practitioner reference for the Anthropic CCA-F certification, built in Q2 2026, covering all five exam domains across 12 chapters.
- [state-of-ai-observability-2026](https://github.com/vkorost/state-of-ai-observability-2026): a Q2 2026 survey of the state of AI observability in production, using Datadog as the main example.
- [sklyarov-hancock-book](https://github.com/vkorost/sklyarov-hancock-book) (Same Stones, Different Gods): comparing Graham Hancock's and Andrey Sklyarov's frameworks on megalithic anomalies. Figuring out how it is possible for two highly intelligent researchers to look at the same exact things and come up with entirely different conclusions.
- [alternative-theories-almanac](https://github.com/vkorost/alternative-theories-almanac): a Q1 2026 survey of the alternative-theory field, 36 chapters, each covering a corresponding area of alternative history.
- [musks-accelerando](https://github.com/vkorost/musks-accelerando): Elon Musk's technological vision mapped onto Charles Stross's 2005 novel Accelerando across 12 concept pairs.

## Tools I built to collect the data for the book projects

These tools have one purpose: produce data in Markdown for easy LLM digestion.

- [site2vault](https://github.com/vkorost/site2vault): mirrors any website into a linked Obsidian vault with a machine-readable manifest for section-level agent reads.
- [obsidian-site2vault](https://github.com/vkorost/obsidian-site2vault): Obsidian plugin that wraps the site2vault CLI and streams crawl progress into a log view.
- [pdf2md](https://github.com/vkorost/pdf2md): PDF to Markdown, auto-routing per page between text extraction and OCR; batch mode.
- [ebook2md](https://github.com/vkorost/ebook2md): EPUB, PDF, FB2, and DJVU to clean Markdown, in batch.
- [ytubefetch](https://github.com/vkorost/ytubefetch): Windows app for batch-downloading YouTube subtitles as AI-ready transcripts. Also fetches audio and video if needed.

## MCP servers

Embedded HTTP servers that expose a running desktop application's UI to AI agents as structured JSON: the desktop equivalent of browser DevTools.

- [java-swing-mcp](https://github.com/vkorost/java-swing-mcp): structured agent access to any Java Swing application: component tree, element state, executable actions, screenshots, and WCAG contrast checks.
- [wpf-mcp](https://github.com/vkorost/wpf-mcp): the same pattern for WPF via the UI Automation API; built to develop and debug [ytubefetch](https://github.com/vkorost/ytubefetch).

## Daily report

A self-running daily news briefing and the comedian voices it closes with.

- [claude-daily-news-report](https://github.com/vkorost/claude-daily-news-report): a Claude Code pipeline that fetches eight news sources, filters them through editorial rules, and assembles a structured daily briefing, capped with a rotating comedian's take on the day's news; runs unattended on a schedule.
- [claude-standup-skills](https://github.com/vkorost/claude-standup-skills): seven comedian-voice Claude skills that supply the briefing's closing monologue, one voice per day on rotation; the report reads them automatically when installed and still runs without them.

## Lightroom plugins

- [lightroom-auto-settings-plugin](https://github.com/vkorost/lightroom-auto-settings-plugin): batch-applies Transform Auto and Auto Settings in Lightroom Classic, an action Adobe never exposed to the SDK; run on every new set of photos.
- [lightroom-geotag-timeline-plugin](https://github.com/vkorost/lightroom-geotag-timeline-plugin): adds GPS coordinates and location names (city, state, country) to photos using your Google Timeline location history, this is for people who have cameras without built-in GPS.

## Audio

A small audio toolchain. Each tool stands alone; chained together they turn a folder of MP3s into a finished offline radio station.

- [mp3-norm](https://github.com/vkorost/mp3-norm): loudness-normalize a folder (EBU R128) so no track is louder or quieter than the next.
- [mp3-trim](https://github.com/vkorost/mp3-trim): detect where the music ends and cut the trailing non-music (talk, applause, dead air) off the tail of each file; music in the middle is left untouched.
- [mp3-radio](https://github.com/vkorost/mp3-radio): the capstone. Turns a folder of MP3s into an offline radio station: writes a comedian-voiced DJ intro for every track, renders each to speech, and assembles an ordered folder any screenless player can play. Uses [claude-standup-skills](https://github.com/vkorost/claude-standup-skills) for the rotating DJ personas.

## A note on platforms

Everything here exists because I needed it and I use all of it, but only on my own setup: Windows and Android, plus the readers and tablets I own. None of it has been tested on macOS, iOS, Linux or other platforms. If you want to run one of these somewhere I have not, the quickest route is to hand the repo to Claude Code, Codex, or whatever agent you use and have it adapt the project to your environment.

---

These are personal projects. The views and work here are my own and unrelated to my past, present and future employers.
