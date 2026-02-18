# TODO: Finish Setting Up Your Website

## Step 1: Preview the Site
- Visit https://joshuakalla.github.io and make sure everything looks good
- Check: Home page shows your photo, bio, and social links
- Check: "Research" page lists all your papers with correct links
- Check: "CV" link opens/downloads your PDF

## Step 2: Review Your Bio
- Open `_pages/about.md` and make sure the bio text is accurate
- If you want to change it, edit the text and push to GitHub

## Step 3: Review Your Research Page
- Open `_pages/research.md` and make sure all papers are correct
- Check that links to papers and replication data work

## Step 4: Point joshuakalla.com to the New Site
Once you're happy with the preview:

1. Tell Claude to "add the CNAME back" (or create a file called `CNAME` in the repo root containing just `joshuakalla.com`)
2. Go to your domain registrar (wherever you bought joshuakalla.com)
3. Update DNS records:
   - DELETE any existing A records or CNAME records for the root domain
   - ADD four A records pointing to:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - ADD a CNAME record: www -> joshuakalla.github.io
4. Wait 30-60 minutes for DNS to propagate
5. Go to https://github.com/joshuakalla/joshuakalla.github.io/settings/pages
6. Check "Enforce HTTPS"

## Step 5: Delete This File
Once everything is set up, you can delete this TODO.md file.
