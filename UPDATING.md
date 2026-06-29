# Updating Your Website

All changes auto-deploy within ~2 minutes of saving to GitHub.

---

## Add a new paper

Edit `data/papers.yaml`. Add an entry under the appropriate section (`articles`, `working_papers`, or `public_writing`):

```yaml
- title: "Your Paper Title"
  authors: "Stark, Liz"
  year: 2026
  status: "working paper"   # or: published, forthcoming
  venue: "Journal Name"     # leave blank for working papers
  url: ""                   # link to PDF or publisher page, or leave blank
```

## Update your bio

Edit `content/_index.md`. The text there is what appears in the About section.

## Add a teaching entry

Edit `data/teaching.yaml`. Add to the `ta` list for TA courses, `lectures` for guest lectures.

## Update your CV

Replace `static/files/cv.pdf` with the new version. Keep the filename exactly as `cv.pdf`.

## Change your photo

Replace `static/images/photo.jpg` with the new image. Keep the filename exactly as `photo.jpg`.

## Mark a paper as published

In `data/papers.yaml`, change `status: "working paper"` to `status: "published"` and add the `venue` and `year` fields.

## Change your email or social links

Edit `hugo.yaml` — find the `params:` section near the top.

## Add a new menu item

Edit `hugo.yaml` — find the `menu:` section and add an entry with `name`, `url`, and `weight` (controls order).
