# Sonar

Sonar is a media-monitoring service that reads public news feeds and article
pages from Mexican outlets for research purposes.

User agent: Sonar/1.0 (+https://github.com/delta-urbano/sonar-bot)

What it does
- Reads RSS/Atom feeds about once an hour.
- Fetches the text of individual articles that match its topics, at most one
  page at a time per site, with a pause between requests.
- Honors robots.txt. Never logs in, never bypasses paywalls, never collects
  comments or personal data. Stores extracted text only, deleted after 30 days.

To block it, add `User-agent: Sonar` to your robots.txt, or write to:
soporte@deltaurbano.com
