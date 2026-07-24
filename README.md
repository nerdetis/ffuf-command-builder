# ffuf command builder

A single-file, no-backend web form that builds ffuf commands from dropdowns and inputs instead of hand-typing CLI flags. Fill in the form, copy the generated command, paste it into your terminal.

Nothing here executes anything — it's just a form that assembles a text string. No server, no dependencies, works straight from the file or from GitHub Pages.

# Why

Typing out ffuf flags from memory is easy to get wrong... especially matcher/filter syntax (-fs, -mc, -fl...) where a typo just silently changes what gets filtered. This turns flag construction into filling out a form instead.

# Usage

Open index.html in any browser — locally, on a shared network drive, or via GitHub Pages. No install, no build step.

Set method, protocol, and target host/path
Add one or more wordlists (supports ffuf's multiple fuzz-point syntax — FUZZ, FUZZ2, etc. — with clusterbomb/pitchfork mode)
Fill in headers, cookies, or POST body as needed
Set any filters/matchers to narrow results
Expand "Advanced options" for proxy, rate limiting, timeouts, etc.
Copy the command from the box at the top (it stays pinned while you scroll)

# Notes
All fields are client-side only — nothing is sent anywhere, nothing is saved between sessions
Wordlist path suggestions assume a typical Kali/Parrot seclists install path; edit the <datalist> in index.html if yours differs
