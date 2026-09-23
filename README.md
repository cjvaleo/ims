# IMS Exteriors website

Website for IMS Exteriors (Landscaping & Lawn Care, Ocean & Monmouth County, NJ).
Plain HTML with no build step. Upload the files as-is and it works.

## What's in here

| File | What it is |
| --- | --- |
| `index.html` | The whole website |
| `images/` | Job photos used on the site |
| `logo/` | IMS patch logo (green and light versions) |
| `CNAME` | Tells GitHub Pages the domain is www.imslandscaping.com |
| `robots.txt`, `sitemap.xml` | Help Google find the site |

## Put it on GitHub

1. Go to github.com, click **New repository**, name it `ims-exteriors-site`, make it **Public**, and click **Create repository**.
2. Click **uploading an existing file**. Drag in everything from this folder (the `images` and `logo` folders too), then click **Commit changes**.
3. Go to **Settings → Pages**. Under "Branch," pick `main` and `/ (root)`, then click **Save**.
4. Wait about a minute. The site shows up at `https://YOUR-USERNAME.github.io/ims-exteriors-site/`.

## Point imslandscaping.com at it

In **Settings → Pages → Custom domain**, enter `www.imslandscaping.com` and save.
Then, wherever the domain was bought (GoDaddy, Namecheap, Squarespace, etc.), change the DNS:

- **CNAME** record: name `www` → value `YOUR-USERNAME.github.io`
- **A** records for the bare domain (`@`), pointing to GitHub:
  `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

After it connects, tick **Enforce HTTPS** in Settings → Pages.
Note: switching DNS takes the current site offline and puts this one up.

## Test the text button

Open the live site on your phone, fill out the quote form, and send a test text to yourself.
The number it texts is set in `index.html`. Search for `17322323429` to change it.
