# Multiverse Global Records (MGR) – site bundle

```
/mgr/index.html        main MGR site (loads css/, js/, assets/)
/mgr/calendar.html     Multiverse calendar (opened inside MGR in a frame)
/mgr/ranking.html      Awards, ranks & badges (opened inside MGR in a frame)
/mgr/assets/           images + anthem audio (audio is the original, uncompressed)
/mgr/css, /mgr/js      styles and scripts, split out of the old single file
/pyramid/index.html    Educational Hierarchy pyramid
```

Notes
- Open through a web server (GitHub Pages, or `python3 -m http.server`), not by double-clicking the file.
- Each page uses its own saved-data key prefix (`mrg_…` for MGR, `pyramid_…` for the pyramid). Give any new page its own prefix, e.g. `school_…`.
- Do not commit real student/staff data to a public repo.
- The ranking page connects to a Supabase project with a *publishable* key. That is safe to be public only if Row Level Security is ON for every table.
- Fonts and the pyramid's QR library load from the internet; the sites need a connection for those.
