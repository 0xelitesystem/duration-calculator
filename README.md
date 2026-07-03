# Duration Calculator

Exact time between two dates, business day counts with holiday exclusions, and add or subtract durations from any date, all in a single HTML file.

**Live demo:** https://0xelitesystem.github.io/duration-calculator/

## Use

- **Difference:** pick a start and an end. You get a calendar-aware breakdown (years, months, days, hours, minutes, seconds) plus exact totals in weeks, days, hours, minutes and seconds. If the end comes first, the tool shows the absolute difference and says so.
- **Business days:** pick two dates and get the count of Monday to Friday days between them. By default the start date is excluded and the end date is included (the "working days until the deadline" convention); both are toggleable. Paste holidays (one YYYY-MM-DD per line) and they are skipped when they land on a counted weekday.
- **Add / subtract:** start from any date and time, then add or subtract years, months, weeks, days, hours, minutes and seconds. Month math clamps to real month lengths, so Jan 31 plus 1 month lands on Feb 28 (or Feb 29 in a leap year).

Every result has a copy button. All math runs in UTC wall-clock space, so answers do not shift with your time zone or daylight saving rules.

## Why this exists

Most date calculators online are ad-farms that send your inputs to a server and bury the answer under trackers. This one is a single MIT-licensed HTML file with zero dependencies, zero network calls and zero surveillance. Read the source in one sitting, verify the math, keep a copy.

## Privacy

Everything runs in your browser. No analytics, no cookies, no fonts or scripts fetched from anywhere, no network requests of any kind. Nothing you type leaves your machine.

## Run locally

```
git clone https://github.com/0xelitesystem/duration-calculator.git
cd duration-calculator
```

Then open `index.html` in any browser, or serve it:

```
python -m http.server
```

## Build

There is no build step. One file, inline CSS and JavaScript, nothing to install.

## License

MIT. See [LICENSE](LICENSE).
