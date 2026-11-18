# shelton-cq-xu.github.io

Personal academic website of Chenqin Xu: <https://shelton-cq-xu.github.io>

Built with [Jekyll](https://jekyllrb.com) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template and hosted on
GitHub Pages. Every push to `master` rebuilds the site within a few minutes.

## Where things are

| What you want to change | File |
|---|---|
| Home page text (bio, interests, ongoing work, contact) | `_pages/about.md` |
| A paper | one file per paper in `_publications/` |
| CV shown on the CV page | `files/CV_Chenqin_Xu.pdf` |
| Sidebar (name, affiliation, email, links, photo) | `author:` block in `_config.yml` |
| Menu at the top | `_data/navigation.yml` |
| Order and titles of the publication groups | `publication_category:` in `_config.yml` |

Leave `_layouts/`, `_includes/`, `_sass/` and `assets/` alone unless you want to change the design.

## Add a paper

Create a new file in `_publications/`, named `YYYY-MM-DD-short-name.md`, with this content:

```markdown
---
title: "Title of the Paper"
collection: publications
category: preprints            # conferences | manuscripts | preprints
permalink: /publication/YYYY-MM-DD-short-name
date: YYYY-MM-DD
authors: "<b>Chenqin Xu</b> and Coauthor Name"
venue: "arXiv:XXXX.XXXXX"      # or the conference / journal name
note: "Under review."          # optional; delete the line when there is nothing to add
arxivurl: "https://arxiv.org/abs/XXXX.XXXXX"   # optional, shown as [arXiv]
paperurl: "https://..."                        # optional, shown as [paper]
codeurl: "https://github.com/..."              # optional, shown as [code]
citation: "Xu, C. and Coauthor, N. (2026). Title of the paper. Venue."
---

**Abstract.** Text of the abstract.
```

The paper then appears on the home page and on the Publications page automatically. Within a group,
papers are ordered by `date`, newest first.

When a preprint is accepted, edit its file: change `category`, `venue`, `note`, `citation`, and add
`paperurl`. Do not rename the file, so the paper's address stays the same.

## Update the CV

Compile the CV on Overleaf, download the PDF, and save it over `files/CV_Chenqin_Xu.pdf` (same file
name). The copy on the website omits the phone number.

## Add a photo

Put the image in `images/`, then set `avatar: "your-file.jpg"` in the `author:` block of `_config.yml`.

## Add a link to the sidebar

Fill in the matching line of the `author:` block in `_config.yml`, for example `googlescholar:` with
the address of the profile. Lines left blank are not shown.

## Add a page to the menu

Listing pages for talks and teaching already exist at `/talks/` and `/teaching/`. To use one, add
entries to a `_talks/` or `_teaching/` folder and add the page to `_data/navigation.yml`.

## Publish a change

```bash
git add -A
git commit -m "Describe the change"
git push
```

Then wait a few minutes and reload the site. The build status is under the repository's Actions tab.
Changes to `_config.yml` are picked up like any other change.
