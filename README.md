# lionsmaneguide.org

Static site, deployed to Vercel from this repo.

## Publishing

Drop a post as `blog/scheduled/<slug>/index.html`. The workflow in
`.github/workflows/publish-scheduled.yml` runs weekly, promotes the oldest
queued folder into `blog/<slug>/`, adds its card to `blog/index.html` and its
entry to `sitemap.xml`, and pushes. The push is the deploy.

Queue depth and the age of the newest post are watched on the microsite
dashboard at `Business/CEO/microsites.html` in the AHARA folder.
