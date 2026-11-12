# 🧩 Unraid templates

Docker templates for [Community Applications](https://ca.unraid.net) by chrizantoz.

| app | what it is | template |
|---|---|---|
| 🩺 [Auditarr](https://github.com/chrizantoz/auditarr) | nightly quality control for a Sonarr / Radarr / Bazarr / Plex library | [auditarr.xml](auditarr.xml) |
| 💾 [Dedupearr](https://github.com/chrizantoz/dedupearr) | the truth about your storage: hardlinks, second copies, leftovers and orphans explained per file, with the evidence | [dedupearr.xml](dedupearr.xml) |

**Until it appears in Community Applications:** Unraid → Docker tab → Template Repositories → add `https://github.com/chrizantoz/unraid-templates` → Save, then Add Container and pick Auditarr or Dedupearr from the list.

The media path is the one thing to get right: mount your media at the same path Sonarr and Radarr use, so the paths they report exist inside Auditarr. Dedupearr needs the library **and** the download folders through one mount, read-only. The [install guide](https://github.com/chrizantoz/auditarr/blob/main/docs/INSTALL.md) has the details.
