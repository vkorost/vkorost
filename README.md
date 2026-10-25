## Books built with Claude Code

I wanted a long, up-to-date read on each of these subjects, could not find one, so I had to build it.

- [weekend-diy-book](https://github.com/vkorost/weekend-diy-book) (Claude Code: The Definitive Guide): a technical book on agentic development with Claude Code, written by Claude Code. Includes the assignment file that produced it, so you can generate your own.
- [claude-certified-architect-guide](https://github.com/vkorost/claude-certified-architect-guide): a practitioner reference for the Anthropic CCAR-F certification, the Foundations tier, built in Q2 2026, covering all five exam domains across 12 chapters.
- [claude-certified-architect-professional-guide](https://github.com/vkorost/claude-certified-architect-professional-guide): a practitioner guide for the Anthropic CCAR-P certification, the Professional tier above CCAR-F, built in Q3 2026, covering all 38 objectives across seven exam domains in 21 chapters.
- [claude-certified-developer-guide](https://github.com/vkorost/claude-certified-developer-guide): a practitioner guide for the Anthropic CCDV-F certification, built in Q3 2026, where a third of the exam turns out not to be about Claude at all.
- [google-certified-ai-leader-guide](https://github.com/vkorost/google-certified-ai-leader-guide): a practitioner guide for Google Cloud's Generative AI Leader certification (GAIL), built in Q4 2026, covering all 15 objectives across the four exam sections, where three of those objectives have no product documentation behind them at all.
- [forward-deployed-engineer-2026](https://github.com/vkorost/forward-deployed-engineer-2026): a Q2 2026 conversion manual for the Forward Deployed Engineer role, ten chapters covering what the work is, the interview architecture, and the conversion path from three adjacent roles (software developer, project manager, engineering manager).
- [ai-risk-field-guide](https://github.com/vkorost/ai-risk-field-guide): an introduction to the AI risk debate, p(doom) and human extinction, drawn from multiple books, essays and articles as of Q3 2026, packaged as an easy-to-digest ebook.
- [tracing-edge-book](https://github.com/vkorost/tracing-edge-book) (Tracing the Edge: What Trading Books Leave Out): a Q2 2026 survey of trading edges in the public record, 14 chapters across four parts, sorting strategies by mechanism — who is on the other side of the trade and whether the edge survived being written down.
- [state-of-ai-observability-2026](https://github.com/vkorost/state-of-ai-observability-2026): a Q2 2026 survey of the state of AI observability in production, using Datadog as the main example.
- [wispr-flow-field-guide](https://github.com/vkorost/wispr-flow-field-guide): a 24-chapter independent reference on Wispr Flow voice dictation, covering the dictation model's mechanics, cleanup engine, command mode, context awareness, coding workflows, and platform-specific setup.
- [healthspan-book](https://github.com/vkorost/healthspan-book) (Healthspan, Annotated): a graded survey of the healthspan and longevity field drawn from ~8,900 videos across 13 podcast channels, 16 chapters sorting claims by who said them and how much weight each one can bear.

## Tools I built to collect the data for the book projects

These tools have one purpose: produce data in Markdown for easy LLM digestion.

- [site2vault](https://github.com/vkorost/site2vault): mirrors any website into a linked Obsidian vault with a machine-readable manifest for section-level agent reads.
- [obsidian-site2vault](https://github.com/vkorost/obsidian-site2vault): Obsidian plugin that wraps the site2vault CLI and streams crawl progress into a log view.
- [pdf2md](https://github.com/vkorost/pdf2md): PDF to Markdown, auto-routing per page between text extraction and OCR; batch mode.
- [ebook2md](https://github.com/vkorost/ebook2md): EPUB, PDF, FB2, and DJVU to clean Markdown, in batch.
- [ytubefetch](https://github.com/vkorost/ytubefetch): Windows app for batch-downloading YouTube subtitles as AI-ready transcripts. Also fetches audio and video if needed.
- [mp3-transcribe](https://github.com/vkorost/mp3-transcribe): local transcription of audio where subtitles are not available, with each speaker labeled.

## Laser dry-fire training

A game, and the book-length research that came before it. The book surveys everybody else's products; the app is what I built after reading it.

- [screenplink](https://github.com/vkorost/screenplink): a laser dry-fire shooting game where the target is the matte monitor you already own. A 60fps webcam watches the screen from one side, and a laser trainer pistol leaves bullet holes where you hit. Nine drills, a seventeen-round magazine, a score that is points per second, and a two-player split screen.
- [laser-dry-fire-field-guide](https://github.com/vkorost/laser-dry-fire-field-guide) (Laser Training for Home Shooters): a Q4 2026 survey of the laser dry-fire category across 16 chapters: the apps, the targets, the sensors and what the scoring and the timers actually measure. Built from vendor documentation and owner reports, with every claim traced to the page it came from.

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
