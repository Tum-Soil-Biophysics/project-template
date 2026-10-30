# First steps: putting your code on the SBE GitHub

This page is for first-time users. Delete the `docs/` folder from your own repository once you are done.

## 1. Create your repository from this template

- This template is a **repository**, not a GitHub "Project". Do not use the **Projects** tab or its *Templates* page. Open https://github.com/Tum-Soil-Biophysics/project-template and click the green **Use this template → Create a new repository** button (top right).
- Owner: **Tum-Soil-Biophysics**. Visibility: **Private**. Name: `Topic_Method`.
- You can also pick it under **New repository → Start with a template → Tum-Soil-Biophysics/project-template**.

**A link shows "404 – Page not found"?** On GitHub this usually means you have no access to a private page, not that it is missing. Check that you accepted the invitation to the organization (https://github.com/Tum-Soil-Biophysics) and are signed in with the right account. Still stuck: contact Prof. Zare (mohsen.zare@tum.de).

## 2. Upload your files

- In your new repository: **Add file → Upload files**.
- You can **drag whole folders** onto the upload page. The folder structure is kept.
- Browser upload limits: **25 MB per file** and **100 files per upload**. Upload in several rounds if needed. Larger files (models, installers, raw data) go to Zenodo or the group drive, not to GitHub.
- Finish each upload with **Commit changes** (bottom of the page).

## 3. Fill in `.zenodo.json`

`.zenodo.json` starts with a dot, so it is a **hidden file** on Windows and macOS. Edit it directly on GitHub: click the file, then the pencil icon (**Edit this file**), then **Commit changes**.

Filled example (Stomify):

```json
{
  "title": "Stomify: a deep learning desktop application for automated stomatal counting",
  "upload_type": "software",
  "description": "Desktop application for automated stomatal counting and density measurement from leaf epidermal impressions, using a YOLOv8m model trained on maize leaf impressions. Belongs to [article]. See README for installation and use.",
  "creators": [
    {"name": "Arachchillage, Vimukthi", "affiliation": "Technical University of Munich"},
    {"name": "Zarebanadkouki, Mohsen", "affiliation": "Technical University of Munich"}
  ],
  "license": "mit",
  "keywords": ["stomata", "stomatal density", "deep learning", "plant phenotyping"],
  "access_right": "open",
  "communities": [{"identifier": "tum-sbe"}]
}
```

Rules: keep the quotes and commas exactly as shown; names as `Family, Given`; replace every `[...]`. Fill in `CITATION.cff` the same way.

**Check your file:** **Actions → Zenodo DOI on release → Run workflow**, enter `v1.0.0`, keep **dry run** ticked, **Run workflow**. A green tick means `.zenodo.json` is fine; a red cross shows what to fix. Nothing is published.

## 4. Release and DOI

You do not release. At acceptance, Prof. Zare makes the repository public and publishes the release; the DOI is then created automatically. If your code **already has a Zenodo DOI**, say so: the automatic release would create a second one.
