# Cal Howland — academic website

A plain HTML/CSS site (no Jekyll, no build step) for GitHub Pages.

```
index.html        Home: photo, bio, CV + Teaching buttons, papers with drop-down abstracts
teaching.html     Teaching portfolio
style.css         All styling (colours are variables at the top)
images/           profile.jpg goes here
files/            CV, drafts, syllabi, statements (PDFs) go here
.nojekyll         Tells GitHub to serve the files as-is
```

## Put it online Instructions ##
1. Sign in at github.com and click **New repository**.
2. Name it exactly `YOUR-USERNAME.github.io` (e.g. `calhowland.github.io`). Set it to **Public**. Create it.
3. On the new repo page, click **uploading an existing file**. Drag in everything from this folder
   (index.html, teaching.html, style.css, .nojekyll, and the images and files folders). Click **Commit changes**.
4. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
5. After a minute or two the site is live at `https://YOUR-USERNAME.github.io`.

To update later: open the file on GitHub, click the pencil icon, edit, and commit. Changes go live in a minute or so.

## Before you publish

- **Photo:** replace `images/profile.jpg` with your own (square works best; keep the same filename).
- **CV:** add `files/Howland_CV.pdf` (or change the link in both HTML files).
- **Abstracts:** every abstract and course description is a placeholder marked `[Placeholder — …]`. Replace them with your own text.
- **Deference paper title:** "Deference as a Scaffold for Solidarity" is a stand-in working title.
- **Teaching PDFs:** the teaching page links to a statement, evaluations, diversity statement and syllabi in `files/`. Add them with those names, or delete the links you don't want.
- **Course details:** add institution and semesters to each course's grey meta line.

## Adding a paper

Copy one `<article class="entry"> … </article>` block in index.html and edit it. To link a draft instead of
"available on request", put the PDF in `files/` and replace the `<span class="note">…</span>` with:

```html
<a href="files/my-draft.pdf" target="_blank" rel="noopener">Draft (PDF)</a>
```
