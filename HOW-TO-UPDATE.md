# How to Update Your Website

Your website is built from files in this folder. When you change a file and
push it to GitHub, the site automatically rebuilds in 1-2 minutes.

There are two ways to make changes:
- **On GitHub.com** (easiest): Go to https://github.com/joshuakalla/joshuakalla.github.io, navigate to the file, click the pencil icon to edit, then click "Commit changes"
- **On your computer**: Edit the file in this folder, then run these commands in Terminal:
  ```
  cd ~/Desktop/Website-new
  git add -A
  git commit -m "describe your change"
  git push
  ```

---

## Add a New Publication

1. Open `_pages/research.md`
2. Add a new line in the right section (Working Papers or Journal Articles)
3. Follow this format:

```
Kalla, Joshua and Coauthor Name. "Paper Title." *Journal Name* (Year). [Paper](URL) | [Replication Data](URL)
```

Just leave out `[Paper](URL)` or `[Replication Data](URL)` if you don't have one of those links yet.

---

## Update Your CV

1. Download your latest CV PDF from Overleaf
2. Rename it to `Kalla_CV.pdf`
3. Replace the file at `files/Kalla_CV.pdf` in this folder
4. Push to GitHub:
   ```
   cd ~/Desktop/Website-new
   git add files/Kalla_CV.pdf
   git commit -m "Update CV"
   git push
   ```

Or on GitHub.com: Go to the `files` folder, click "Add file" > "Upload files", upload `Kalla_CV.pdf`, and commit.

---

## Update Your Bio (Home Page)

Edit `_pages/about.md`. The text below the `---` block is what appears on your home page.

To change the one-line bio that appears in the sidebar under your photo, edit the `bio` line in `_config.yml`.

---

## Move a Paper from Working Papers to Journal Articles

Just cut the line from the "Working Papers" section and paste it into the "Journal Articles" section in `_pages/research.md`. Update the citation to include the journal name and year.

---

## Change Your Photo

1. Put the new photo in the `images/` folder
2. In `_config.yml`, change the `avatar` line to match your new filename:
   ```
   avatar: "new-photo-name.jpg"
   ```

---

## File Reference

| File | What it controls |
|------|-----------------|
| `_pages/about.md` | Home page bio text |
| `_pages/research.md` | Research page (all papers) |
| `files/Kalla_CV.pdf` | Your CV PDF |
| `images/Headshot.jpg` | Your profile photo |
| `_config.yml` | Site title, sidebar bio, social links, email |
| `_data/navigation.yml` | Top navigation bar links |
