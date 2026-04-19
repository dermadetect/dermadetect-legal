# dermadetect-legal

Static content served at **https://privacy.dermadetect.com** via GitHub Pages.

## What's here

- `index.html` — DermaDetect privacy policy at https://privacy.dermadetect.com/
- `account-deletion/index.html` — account deletion instructions at https://privacy.dermadetect.com/account-deletion/ (required by Google Play)
- `CNAME` — GitHub Pages custom domain binding

## How it's served

- GitHub Pages publishes the `main` branch from the root of this repo
- The `CNAME` file binds the site to `privacy.dermadetect.com`
- DNS for `privacy.dermadetect.com` lives in the `env-secure` Terraform environment in the `dermadetect/terraform` repo as a CNAME to `dermadetect.github.io`

## Updating the policy

1. Edit `index.html` directly on `main` (or via PR) — GitHub Pages rebuilds automatically
2. Update the "Last updated" date in the header
3. Verify at https://privacy.dermadetect.com after a minute or two
