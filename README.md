# Parser for DTEK-KREM outage schedule

The latest data is available at `dtek_data.json` in the `data` branch.

## Other sites

To adapt this parser for additional DTEK sites, follow these steps:

- Fork the repository.
- Update the `url` variable in `scraper_github_actions.py` to point to the desired site.
- Obtain a free [browserless](https://www.browserless.io/) account and copy your token.
- In the repository’s Security → Secrets and variables settings, add a new Actions secret named `BROWSERLESS_TOKEN` and paste the token.
- (Optional) Set a `WEBHOOK_URL` secret if you want the latest JSON posted to an external endpoint whenever the schedule changes.
- Enable scheduled GitHub Actions.
- You’re all set!
