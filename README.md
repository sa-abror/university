# HTML Review — Lab Work 3

A nine-page HTML and CSS website with **86 tag guides**. Each guide includes a
definition, an `Attribute` / `Role` table, escaped HTML source in `<pre><code>`,
and the same example rendered in the browser.

Repository: <https://github.com/sa-abror/university>.

## Run locally

Open this folder in VS Code. Install the **Live Server** extension, right-click
`html_review/index.html`, and choose **Open with Live Server**. Alternatively,
run the following command from the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000/html_review/>. No build, JavaScript framework, package
installation or backend is needed. Use a local HTTP server so the browser can
load the video's WebVTT captions reliably.

## Files

```text
university/
├── README.md
├── .gitignore
├── .nojekyll
├── index.html                # GitHub Pages entry; opens html_review/index.html
└── html_review/
    ├── index.html            # 01 — Home and document structure
    ├── text.html             # 02 — Text formatting
    ├── links.html            # 03 — Links, images, audio and video
    ├── lists.html            # 04 — Lists
    ├── tables.html           # 05 — Tables
    ├── forms.html            # 06 — Forms
    ├── media.html            # 07 — Multimedia
    ├── semantic.html         # 08 — Semantic and layout elements
    ├── metadata.html         # 09 — Metadata
    ├── css/style.css         # The single shared external stylesheet
    └── images/
        ├── study-desk.svg
        ├── study-desk-small.svg
        ├── favicon.svg
        ├── video-poster.svg
        ├── chime.wav
        ├── html-demo.webm
        └── captions.vtt
```

## Assignment coverage

| Requirement | Implementation |
| --- | --- |
| Nine linked pages | All nine chapters are in `html_review/` |
| Definition, Attributes, Example | 86 guides with source and live output |
| Two-column attribute tables | `Attribute` and `Role` column headings |
| Escaped source code | `<pre><code>` using `&lt;`, `&gt;` and other entities |
| Shared header, navigation and footer | Same layout and menu, with current-page indication |
| One external stylesheet | `css/style.css`; no inline styles or style tags |
| Selectors, colours, box model, Flexbox | Responsive navigation, chapter cards and example panels |
| Local images, audio and video | Original bundled assets, with captions and text descriptions |
| Pages publication entry point | Root `index.html` forwards to the website |

Document-root, `main` and metadata examples use separate HTML documents inside
`iframe srcdoc`. The displayed source and the embedded document match. Metadata
that has no visible output has an explanation of its effect.

The form demonstration submits a sample topic back to `forms.html` using GET,
so the value appears in the address bar. This static site does not process or
store submissions. Native input validation, reset, checkboxes, radio buttons,
selects and expandable `details` examples work without JavaScript.

## Publish with GitHub Pages

In the repository's **Settings → Pages**:

1. Set **Source** to **Deploy from a branch**.
2. Select **main** and **/(root)**, then click **Save**.
3. Wait for the Pages deployment to succeed and open the published website.

Expected address after publication:
<https://sa-abror.github.io/university/>.
This address is not a claim that Pages has already been enabled.

The root entry page lets Pages serve the existing `html_review` folder.
[GitHub's documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
explains the available branch publishing sources.

For future updates, commit and push through the IDE, or run:

```sh
git add README.md index.html .gitignore .nojekyll html_review
git commit -m "Update HTML review website"
git push origin main
```

## Remaining submission details

- Add both students' full names and the partner's GitHub username to this README.
- In **Settings → Collaborators → Add people**, invite the partner. They must
  accept the invitation.
- Invite the teacher using **info.moumni.nourchen@gmail.com**, as requested in
  the assignment. The teacher must accept the invitation.
- The assignment specifies a repository named `html-review` and an outer folder
  named `Project_fullname1_fullname2`. This implementation preserves the supplied
  `university` repository and the existing `html_review` source folder. Confirm
  the naming with the teacher before submission. If the exact names are required,
  rename the repository in GitHub Settings and update the remote, repository
  links and published URL. Rename the local outer folder using the real names
  of the two students; relative website links will continue to work.

Repository settings and invitations require owner access. The local files do
not enable Pages or send invitations automatically.

## Verification

- All nine chapters and the root entry pass HTML Validate.
- Chrome checks cover all 86 code/result pairs, attribute tables, local links,
  unique IDs and shared navigation, header and footer.
- Layout checked at 320, 390, 768 and 1440 pixels without horizontal page overflow.
- Tested GET submission, reset, input validation, label focus, checkboxes,
  keyboard-controlled disclosures, audio/video playback, captions and responsive
  images.

Before submission, also open the pages with Live Server as requested in the
assignment and check the published Pages URL.

## Assets and references

The vector illustrations, icon, three-note audio chime, six-second silent video
and captions were created for this project and are stored locally. No external
fonts, hosted images or third-party video players are needed.

HTML reference: [WHATWG HTML Living Standard](https://html.spec.whatwg.org/multipage/).
The brief W3C quotation in the text chapter cites the
[W3C mission page](https://www.w3.org/mission/).
