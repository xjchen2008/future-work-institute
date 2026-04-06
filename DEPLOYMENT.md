# Deployment Notes

## Current existing website flow

Existing static site folder in active use:
`/Users/james/Library/CloudStorage/Dropbox/Career/skyworks/on_site_2026/cloudflare_publish_v1`

That folder appears to be:
- a git-backed static website
- manually editable
- suitable for Cloudflare/static publishing

## Recommended deployment strategy for Future Work Institute

Because the current site is James's RFIC portfolio, the cleanest approach is:

### Option A — Separate site (recommended)
Create a new publish folder/repo for Future Work Institute, for example:
`/Users/james/Library/CloudStorage/Dropbox/Career/future_work_institute/site_v1`

Benefits:
- does not overwrite the existing portfolio
- easier branding and domain separation
- cleaner deployment history

### Option B — Subdirectory in existing site
Add Future Work Institute under a subdirectory such as:
`/future-work-institute/`

Benefits:
- fast prototype
- reuses current deployment flow

Tradeoff:
- couples two unrelated websites together

## Suggested next implementation step

1. Create a dedicated deploy folder
2. Copy `index.html` and any future assets into it
3. Initialize or connect git if needed
4. Deploy to Cloudflare Pages / worker-backed static hosting / existing publishing flow

## What I mean by CTA sections

CTA = call to action.
Examples:
- `Apply as a Builder`
- `Join the First Cohort`
- `Request Early Access`
- `Hire a Ranked Operator`

## What I mean by application forms

These are simple forms on the landing page that let users do something concrete, such as:
- builders applying to submit an operator
- companies requesting early access
- users joining a waitlist

For now, the current website draft does not need forms yet. The better immediate task is deployment plumbing.
