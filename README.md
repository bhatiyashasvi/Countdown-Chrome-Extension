# Countdown-Chrome-Extension
A minimalist Chrome extension that replaces your new tab with a live countdown timer. Inspired by YC founders counting down to Demo Day.

## Features
- Live countdown — days, hours, minutes, seconds updating every second
- Dark / Light / Auto theme — toggle with one click, follows system preference by default
- Theme persistence — remembers your choice across sessions
- Zero clutter — no analytics, no tracking, no permissions, no frameworks
- Fully customizable — change the title, quote, deadline, anything

## Build-Your-Own-Countdown
Open Claude and just copy paste my prompt into your Claude. Make sure to edit the inputs like deadline date and time, title, any quote if you want, etc 

### Prompt
Build me a complete Chrome New Tab Extension that replaces my default new tab page with a live countdown timer. I need you to generate all the files as a downloadable package (.zip) that I can install in Chrome via chrome://extensions → "Load unpacked".
### My Inputs
Countdown Title: [YOUR TITLE HERE — e.g., "Days Left to Land a Job"]
Countdown End Date & Time: [YOUR DATE & TIME HERE — e.g., "May 31, 2026 11:59 PM"]
Theme: [PICK ONE: "dark" / "light" / "auto (follow system)"]
Design & Behavior Requirements
New Tab Override — Every time I open a new tab in Chrome, this page should appear instead of the default one.

### Other Settings
Live Countdown — Display a real-time countdown (updating every second) showing:
Days (3-digit padded, e.g., 062)
Hours (2-digit padded, e.g., 03)
Minutes (2-digit padded, e.g., 48)
Seconds (2-digit padded, e.g., 57)
Layout (top → bottom, all centered):


Title — displayed in a bold serif or clean sans-serif font, slightly smaller than the countdown numbers.
Optional subtitle/quote — a small motivational line beneath the title in muted/gray text (use the quote: "You have the right to act. Never to the fruits thereof. — Bhagavad Gita 2.47", or let me customize it).
Countdown numbers — the main visual focus. Medium-large, bold, high-contrast white (dark mode) or black (light mode). Each unit separated by a colon (:) with subtle styling.
Unit labels — tiny uppercase spaced-out labels ("DAYS", "HOURS", "MINUTES", "SECONDS") directly below their respective numbers.
Deadline reminder — a small muted line at the bottom showing the target date & time (e.g., DEADLINE · MAY 31, 2026 · 11:59 PM).
Theming:


Dark mode: Background #121212 or near-black, text white/light gray.
Light mode: Background #FAFAFA or near-white, text dark gray/black.
Auto: Follow the user's system preference via prefers-color-scheme.
Include a small, unobtrusive toggle icon (e.g., sun/moon) in the top-right corner so I can manually switch themes.
Typography & Style:


Use a clean, modern font — system fonts or Google Fonts (e.g., Inter, Space Grotesk, or similar).
Countdown numbers should use a monospace or tabular-number font so digits don't jump around as they change.
Overall aesthetic: minimalist, focused, distraction-free — inspired by the YC Demo Day countdown style.
Smooth fade-in on page load.
No unnecessary borders, shadows, or decorations.
When countdown reaches zero:


Display a congratulatory or completion message (e.g., "⏰ Time's Up!" or "The Day Has Arrived!").
Stop the timer at 00 : 00 : 00 : 00.
Files to generate:


manifest.json — Chrome extension manifest (Manifest V3), with chrome_url_overrides for newtab.
newtab.html — The HTML page.
style.css — All styling.
script.js — Countdown logic, theme toggle, and localStorage persistence for theme preference.
icon.png (16×16, 48×48, 128×128) — Simple countdown/clock icon, or generate a minimal SVG-based one.
A README.md with installation instructions.
Package everything into a .zip file I can download directly.


What NOT to include
No analytics, tracking, or external API calls.
No unnecessary permissions in the manifest.
No frameworks — keep it vanilla HTML/CSS/JS.
No clutter or extra UI elements.

## Deployment Steps-to-follow
1. Open chrome://extensions in Chrome
2. Turn on Developer Mode (top-right toggle)
3. Click Load unpacked → select the extension folder
4. Open a new tab. That's it.



