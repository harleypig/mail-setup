# mail-setup

A friendly, mobile-first help page that walks non-technical users through
setting up their **harleypig.com** mailbox on a phone (IMAP / POP3 / SMTP).

- Single self-contained `index.html` (no build step).
- Served via **GitHub Pages** at <https://mail-setup.harleypig.com>.
- Server settings shown are MXroute's; the branded host `mail.harleypig.com`
  is used (valid after the MXroute cutover + mail-host AutoSSL cert).
- No email addresses or passwords appear on the page — the settings are
  public, non-sensitive values (see the harleydev repo's MXroute docs).

## Hosting

Published from the default branch (`main`, root) — Pages "Deploy from a
branch". `CNAME` sets the custom domain; `.nojekyll` skips Jekyll.

The DNS record (`mail-setup.harleypig.com` → `harleypig.github.io`) lives in
the harleydev infra repo (`domains/yaml/harleypig_com.yml`).
