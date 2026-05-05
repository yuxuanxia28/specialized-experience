# NGA Specialized Experience Prototype

This workspace contains a local recreation of the GitHub Pages prototype at:

https://yuxuanxia28.github.io/specialized-experience/

## Run

```bash
npm start
```

Then open:

```text
http://localhost:4173
```

## NGA API Repo

The provided API repo is cloned in `nga-api/`. It is an older Express/Mongo scraper service with a single app endpoint:

```text
GET /onview
```

If you have its Mongo database configured and the service running on port 3000, this local prototype server can proxy it at:

```bash
NGA_API_URL=http://localhost:3000 npm start
```

The visual prototype remains curated because the original experience depends on hand-authored quadrant positions, relevance scores, tags, descriptions, and explanatory text that are not present in the `nga-api` `/onview` response.
