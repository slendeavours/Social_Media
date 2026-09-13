# The Boardroom Sessions

Event landing page for SL Endeavours Ltd, served at events.slendeavours.org via GitHub Pages.

## Current state

Stage 1 of 5: interest capture only. No price, no dates, no location named, no registration counter.

## Files

- `index.html` - the page
- `crest.png` - SL Endeavours crest, white background removed, for dark backgrounds
- `logo.png` - full lockup with wordmark, used in footer
- `CNAME` - custom domain for GitHub Pages

## Form

HubSpot embedded form.

- Portal: 26792037
- Form GUID: 634aab5c-11e1-4b02-9b30-18504bc49bb2
- Region: eu1

The form will not render when the file is opened locally from disk. HubSpot's embed needs the page served over HTTPS from a real domain. Test on the deployed URL.

## Deploying

1. Push to the repo root on the default branch
2. Settings, Pages, deploy from branch
3. In Cloudflare add a CNAME record: `events` pointing to `slendeavours.github.io`, DNS only
4. Wait for the certificate, then check https://events.slendeavours.org

## Stage changes

Stages are tagged releases so each year's version can be recovered.

- Stage 1 interest: this version
- Stage 2 applications: swap the HubSpot embed for the Jotform to Postgres form, add video, make criteria explicit
- Stage 3 review: no page change, worked in CRM
- Stage 4 selected attendees: no page change, handled in Sender
- Stage 5 post event: add photos and outcomes, reopen interest for the following year

The copy blocks that change between stages are the masthead standfirst, the availability section, and the register section. Everything else carries over.
