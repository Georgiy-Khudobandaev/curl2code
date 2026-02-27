<p align="center">
  <img src="https://raw.githubusercontent.com/Georgiy-Khudobandaev/curl2code/main/og-image.png" alt="curl2code" width="600" />
</p>

<h3 align="center">Convert curl commands to code in 30+ languages — instantly, privately, in your browser.</h3>

<p align="center">
  <a href="https://curl2code.com">curl2code.com</a> &nbsp;|&nbsp;
  <a href="https://curl2code.com/en/contact">Contact</a> &nbsp;|&nbsp;
  <a href="#about-the-author">About Me</a>
</p>

---

## What is curl2code?

**curl2code** is a free web tool that converts curl commands into working code for **31 language families (49 variants)** — Python, JavaScript, Go, Java, PHP, Rust, C#, Swift, Kotlin, Ruby, TypeScript, and many more.

All conversions happen **entirely in your browser** using WebAssembly. Your data never leaves your machine for basic conversions.

Powered by the excellent open-source [curlconverter](https://github.com/curlconverter/curlconverter) library.

> **Note:** The core application is closed-source. This repository serves solely as the official public issue tracker, feature request hub, and a showcase of the project's architecture. You won't find the source code or development history here, but you can explore the tech stack below and interact with the creator.

## Features

**Core**
- **31 language families, 49 variants** — from Python `requests` to Rust `reqwest` to C `libcurl`
- **Client-side conversion** — WebAssembly-powered, zero server round-trips
- **Smart Clean** — strips browser junk headers from DevTools "Copy as cURL"
- **Full Example mode** — adds try/catch, types, error handling, imports

**Tools**
- **cURL Builder** — visual HTTP request constructor with headers, auth, body editor
- **Split View** — compare output in two languages side by side
- **Share links** — short URLs to share curl snippets with generated code

**AI (Bring Your Own Key)**
- **AI Explain** — get a plain-English breakdown of what the curl command does
- **Reverse** — paste code, get the equivalent curl command back
- Supports OpenRouter, OpenAI, Anthropic, Google AI
- Your API key stays in your browser — never stored on our servers

**Internationalization**
- **39 locales** — full UI translation including RTL (Arabic, Hebrew, Farsi, Urdu)
- **1,200+ SEO-optimized language pages** — `/en/python`, `/de/go`, `/ja/rust`, etc.

**Privacy & UX**
- Dark / light / system theme
- GDPR-compliant cookie consent
- No accounts, no sign-ups, no tracking without consent

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js 16 (App Router) |
| Language | TypeScript 5.9 (strict) |
| UI | shadcn/ui + Radix UI + Tailwind CSS 4 |
| State | Zustand 5 |
| Database | PostgreSQL 18 + Prisma 7 |
| Cache | Redis 8 (rate limiting) |
| Conversion | curlconverter (WASM, client-side) |
| AI | BYOK — user's own API key, proxied per-request |
| i18n | next-intl (39 locales) |
| Monitoring | Sentry + PostHog (with consent) |
| Testing | Vitest + Playwright |
| Quality | ESLint 9 + Prettier + Husky + lint-staged |

## 🐞 Feedback & Issues

Have an idea for a new language, or found a bug? Since the application's source code is private, please use this repository's public issue tracker to share your thoughts and help improve the product!

- [🐛 Report a Bug](https://github.com/Georgiy-Khudobandaev/curl2code/issues/new?template=bug-report-description--report-an-issue-or-bug-in-curl2code-template-content-.md)
- [💡 Request a Feature](https://github.com/Georgiy-Khudobandaev/curl2code/issues/new?template=feature-request-description--suggest-an-idea-or-a-new-language-support-for-curl2code-template-content-.md)

## Acknowledgements

This project wouldn't exist without [curlconverter](https://github.com/curlconverter/curlconverter) — an incredible open-source library that does the heavy lifting of parsing curl commands and generating code in dozens of languages. Huge thanks to [Nick Carneiro](http://trillworks.com) and all contributors.

## About the Author

**Georgiy Khudobandaev** — Full-Stack Developer

I build web applications, Telegram bots, and automation tools. curl2code is one of my projects — I enjoy turning complex tasks into simple, well-crafted solutions.

**Always open to collaboration and new projects.**

- Email: [georgiy.khudobandaev@gmail.com](mailto:georgiy.khudobandaev@gmail.com)
- Telegram: [@Georgiy_H](https://t.me/Georgiy_H)
- GitHub: [@Georgiy-Khudobandaev](https://github.com/Georgiy-Khudobandaev)

## License

The curl2code application is proprietary. All rights reserved.

The curl-to-code conversion engine is powered by [curlconverter](https://github.com/curlconverter/curlconverter), licensed under the [MIT License](https://github.com/curlconverter/curlconverter/blob/master/LICENSE).
