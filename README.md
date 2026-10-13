# dataadvisoryllc.com

A small static site for the Data Advisory LLC practice. No build step, no framework — plain HTML and one shared stylesheet, same approach as the caroldavidsen.com site.

## Files

- `index.html` — single page: About the practice, Services (grouped into five categories), and a closing contact band
- `styles.css` — shared styles

## Editing the services list

Each service lives in a `<li>` inside a `<ul class="service-list">`, grouped under a `<div class="service-group">` with its own `<h3 class="section">` heading. To add a service, copy an existing `<li>` block (`service-name` + `service-desc`) within the right group. To add a new group, copy an entire `.service-group` block and give it a new heading.

## Deploying

Same pattern as caroldavidsen.com: connect this repo to Cloudflare Pages (Workers & Pages → Create → Pages → Connect to Git), framework preset "None," no build command, output directory `/`. Point the dataadvisoryllc.com custom domain at it the same way www.caroldavidsen.com was added — a DNS record plus a Workers/Pages domain or route.
