termspy-wiki
============

The wiki component of the termspy gem.

## What is this?

The termspy site when populated will be uploaded to this repository, as it will be a plain old git repository fed by the termspy gem.

This repository is used as the backend to a gollum wiki for administration of the termspy site, and is statically served by the smeagol gem.  This allows for data freedom as it is all just plaintext and can be cloned by anyone who has knowledge of git.

## Layout

This repo is organised as follows.

```
/
- home.md
- /sites
-- github.md
- /terms
-- home.md
-- /github
--- terms-of-service.md
--- privacy-policy.md
```

### Sites

Each site scraped by termspy has a page created in here.  It contains wiki links to the terms pages, which have the source document in a URL link underneath them.  Termspy will scrape the source link and put the formatted results into the heading.

### Terms

The home page under the terms folder acts as an index for all the terms in the wiki.  Then each site is under their own subfolder under terms.
