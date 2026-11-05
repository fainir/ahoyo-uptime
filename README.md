# ahoyo-uptime

Hourly check, from outside Railway, that https://ahoyo.app and its database answer
(`/readyz` checks the database, `/` checks the site). A failed run emails the repo owner,
which is GitHub's default for failed scheduled workflows.

Public on purpose: scheduled Actions in public repos use no paid minutes. Nothing here is secret.
GitHub pauses schedules in a repo with no activity for 60 days; if that happens, re-enable the
workflow under Actions.

Run it now: Actions > Uptime > Run workflow, or `gh workflow run uptime.yml -R fainir/ahoyo-uptime`.
