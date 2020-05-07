---
title: JAMstack Presentation    
marp: true
theme: uncover
align: left
paginate: true
header: MyMiniFactory: JAM Stack
---

# JAM Stack
#### (and bits of Gatsby)

---

# What is the JAM Stack?
#### JavaScript/API/Markdown
Name introduced by Netlify (CDN provider)
- No backend just static HTML/CSS/JS
- Generated Frontend
- Markdown or API for dynamic content
---

<!-- But it gets a bit more interesing -->

# History and problematic
Netlify's CEO was maintaining broken Wordpress
- Having to *maintain* a server (resources, updates, CEVs)
- HTML/CSS in Database problems (Not pure Sementics, Transferability of contents)
- Databases are just slow

<!-- DB are also not scalable -->

---


# Why now?
How is this new?

<!-- pure HTML sites with FTP is not new -->

---

## 1. Static site generators
- Hugo: The fast `Go`
- Gatsby: The full-fledge `React`
- Zola: The frenchy `Rust`

---

## 2. CDN and edge performance
- Cloudflare: 10ms everywhere
- Scalability
- DevOps left to CDN companies

---

# Gatsby
- Using different source of content to build the static site with GraphQL: Markdown, Databases, APIs
- Powerfull pre-fetching / lazyloading

---

# Example: Workflow 
- Content editable by non-devs. (Markdown, CMS)
- Pushed Markdown files to GitHub
- Automatically builds the font

---

# Demo
## Scan The World
- Netflify CMS
- MyMiniFactory API 
- GraphQL local DB 
<!-- Demo: The Netlify CMS commits to Git -->

---

# Limits
- Authentication (On first load/Stateless) (Edge computing?) doesn't solve required DB
- React and SSR: downloading the content twice
(SSR, not specific to JAM)
- Dynamic content with many pages
(How big?)
- Content in git Repo problems: assets, images etc.
<!-- Gatsby a bit slow, Hugo fast -->

---

# Questions?