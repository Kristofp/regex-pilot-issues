<div align="center">

# RegexPilot

**A visual regex builder for macOS that runs your pattern on the real engine.**

[Website](https://regexpilot.com) · [Download](https://regexpilot.com/download) · [Mac App Store](https://apps.apple.com/us/app/regexpilot/id6764146125?platform=mac)

</div>

<img src="https://regexpilot.com/demo-preview.png" alt="RegexPilot editing a regular expression as a railroad diagram, with live match results" width="100%">

---

## What it does

RegexPilot turns a regular expression into a **railroad diagram you can edit directly** — drag blocks from a palette, connect them on a track, and read a plain-English explanation of every part as you work.

## Why it's different

Most regex tools test your pattern with JavaScript and hope it behaves the same in the language you actually ship. RegexPilot **bundles 14 native engines** and runs the pattern through the real interpreter for your target language, so match offsets are byte-identical to production:

| Flavor | Engine |
|---|---|
| Python | CPython (`re` and `regex`) |
| Java | `java.util.regex` via GraalVM |
| Ruby | Onigmo via CRuby |
| C# | .NET |
| PHP | PCRE2 via static-php |
| Go | RE2 |
| PostgreSQL | Spencer |
| MySQL | ICU |

21 flavors in total, including JavaScript, TypeScript, Perl, Rust, Swift, Scala, Kotlin, Groovy, Clojure, Elixir, R, Dart and Shell.

It exists because an AI-generated postal-code regex passed in JavaScript and silently failed in production three days later.

## Other things it does

- **AI-assisted generation** — describe a pattern in English and get a working draft. Bring your own key (OpenAI, Claude, Gemini and others) or run fully offline with Ollama, LM Studio or llama.cpp.
- **Voice dictation** — on-device via a bundled Whisper model, 100 languages.
- **Live testing** — paste sample text, watch matches and capture groups highlight as you type.
- **Pattern library** — 50 curated patterns, plus folders, tags, import and export.
- **Code generation** — copy your pattern as ready-to-paste code in 19 languages.
- **Editor integration** — open patterns from VS Code; quick-test from Raycast or Alfred.
- **Privacy by construction** — no accounts, no telemetry, no cloud calls. The only network request is an AI call you explicitly make with your own key.

## Install

```sh
brew install --cask kristofp/regexpilot/regexpilot
```

Or [download the DMG](https://regexpilot.com/download), or get it from the [Mac App Store](https://apps.apple.com/us/app/regexpilot/id6764146125?platform=mac).

**Requirements:** macOS 14 (Sonoma) or later. Universal binary, signed and notarized.
**Languages:** English, Dutch, French, German.
**Pricing:** free tier covers JavaScript and TypeScript with no time limit; a one-time purchase unlocks all 21 flavors.

---

## Reporting a bug

This repo is the **public issue tracker**. The app's source is private; this exists so bugs and feature requests are visible and trackable.

[Open a bug report](https://github.com/Kristofp/regex-pilot-issues/issues/new?template=bug_report.md)

Please include:

- Your RegexPilot version (Settings → About)
- macOS version
- The regex flavor you were using, if relevant
- Steps to reproduce

## Requesting a feature

[Open a feature request](https://github.com/Kristofp/regex-pilot-issues/issues/new?template=feature_request.md)

## Before you file

- Search existing issues — someone may have reported the same thing
- For urgent account or billing issues, email support@regexpilot.app instead
