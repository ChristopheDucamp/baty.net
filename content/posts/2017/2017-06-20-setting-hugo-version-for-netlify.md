---
title: "Setting Hugo Version for Netlify"
date: 2017-06-20T14:51:09-04:00
tags: ["Netlify","Hugo"]
slug: "setting-hugo-version-for-netlify"
---

After deploying my blog via Netlify I noticed some pieces were missing. Turns
out I needed to tell Netlify which version of Hugo to use during the build.

Adding the following to the netlify.toml file was all it took.

```
[context.production.environment]
  HUGO_VERSION = "0.23"
```
