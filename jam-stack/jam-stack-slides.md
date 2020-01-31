---
title: JAMstack Presentation    
marp: true
theme: uncover
align: left
paginate: true

---

# JAM Stack
#### (and bits of Gatsby)

---

# What is the JAM Stack?
#### JavaScript/API/Markdown
Name introduced by Netlify (CDN provider)
- No backend serving HTML
- Generated Frontend
- APIs only
- M?
---

# How does it work
## Principles:
- Static content that can be served by a CDN

---

# Why?

---

# Servers issues
CMS/Wordpress issues
- Having to maintain a server <br>(ressources, updates, CEVs)
- HTML in Database
---

# Performance
### The great
- Amazing first load: everything is served by a close CDN
- Having to do everything with API calles after can delay things

---

# Content management
- Content in Git repo:
- Commit site content (even non-devs)

For non-devs: Netlify CMS

---

# History
Netlify's CEO was working on many Wordpress

---

# Static site generators
- Hugo `The Fast Gopher`
- Gatsby `The Full Reactive`
- Zola `The Rusty french`

---

# Example: Scan The World 
- Content editable by Jon on a CMS
- Pushed Markdown files to GitHub
- Automatically builds the font

---

# Limits
- Authentication (On first load/Stateless)
- React and the SSR: downloading the content twice
(Not specific to JAM)
- Dynamic content with many pages
(How big?)

---

# Questions?