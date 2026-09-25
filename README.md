# HTML Review — Lab Work 3

A simple first-year project made with HTML and CSS.

## Pages

- `index.html` — page structure
- `text.html` — text formatting
- `links.html` — links, images, audio and video
- `lists.html` — lists
- `tables.html` — tables
- `forms.html` — forms
- `media.html` — multimedia
- `semantic.html` — semantic and layout tags
- `metadata.html` — page information

All nine pages are in `html_review/`. Every tag example includes:
a definition, an Attribute / Role table, HTML code and its browser result.
The six heading levels are shown together in one example.

## How the project works

- The same header, menu and footer are written in each page.
- All CSS is in `html_review/css/style.css`.
- Pictures, audio, video and captions are in `html_review/images/`.
- `html_review/examples/` contains two small example pages. They let us show
  document tags and metadata without putting one HTML document inside another.
- The menu uses Flexbox. There is no JavaScript or framework.
- The sample form sends a topic to the same page with GET. It does not save data.

## Open the site

In VS Code, open `html_review/index.html` with **Live Server**.
Or run this command from the `university` folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8000/html_review/>.
Use a local server so that the video captions can load.

## GitHub and submission

1. Commit and push the finished files in PyCharm or VS Code.
2. In GitHub **Settings → Pages**, select **Deploy from a branch → main → /(root)**.
3. In **Settings → Collaborators**, invite your partner and the teacher:
   **info.moumni.nourchen@gmail.com**. Both must accept their invitations.
4. Add both students' full names to this README before submitting.

The assignment requests the repository name `html-review` and the outer folder
name `Project_fullname1_fullname2`. The supplied repository is currently called
`university`. Confirm the name with the teacher or rename it before submission.
If you rename the repository, also update its links and your Git remote.

After Pages is enabled, the expected site address is
<https://sa-abror.github.io/university/>. The root `index.html` opens the site
in `html_review/`. Pages settings and invitations need the owner's account.

## Quick check before submitting

- Open every page and try the menu links.
- Compare each code example with its result.
- Try the forms, audio and video.
- Resize the browser to check the layout on a small screen.

All media files were made for this project. No external libraries are needed.
