# ARTIZYN Design Studio website

Your current Canva website rebuilt as editable HTML, CSS and JavaScript, with the first Architrexx website's blue-and-black visual system and interactions.

**The brand and company content are Artizyn's current information.** The older Architrexx company text, sample services, older team title, and academic footer have not been added to this version.

## 1. Open and run in VS Code

1. Download and extract `artizyn-website-github.zip`.
2. Open **VS Code → File → Open Folder**.
3. Select the extracted `artizyn-website` folder containing `index.html`.
4. Open `index.html` in your browser, or use **Open with Live Server** if that VS Code extension is available.
5. Edit a file, save it, and refresh your browser. Live Server refreshes the page automatically.

No Node.js, npm installation, API key or build command is required. You can double-click `index.html` from File Explorer to preview it. The local site includes its own photos, portraits and video. The third-party chatbot and outbound links need an internet connection.

If you have Python installed, you can also open a terminal in this folder and run:

```bash
python -m http.server 5500
```

Then open `http://localhost:5500`. Stop the server with Ctrl+C.

## 2. Publish through GitHub Pages

VS Code is the editor. **GitHub Pages hosts the live website.** This ZIP is ready to upload, but has not itself been published to your GitHub account.

### Easiest upload method

1. Sign in to GitHub and create a repository, for example `artizyn-website`. For GitHub Free, choose **Public** to use GitHub Pages.
2. In that repository, choose **Add file → Upload files** (or the upload link on a new empty repository).
3. Upload the **contents inside** your extracted `artizyn-website` folder. Upload `index.html`, the seven other HTML files, `styles.css`, `script.js`, and the entire `assets` folder. Do not upload only the ZIP, and do not put the whole site inside an extra nested folder.
4. Commit the uploaded files. Make sure `index.html` appears in the repository's top level.
5. Open **Settings → Pages**.
6. Under **Build and deployment → Source**, choose **Deploy from a branch**.
7. Choose **main** and **/(root)**, then **Save**. If your repository uses a different branch name, choose that branch.
8. Wait for the deployment. Under **Settings → Pages**, use **Visit site** to open the URL GitHub provides. Publishing may take several minutes.

Your project site normally follows the pattern `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`. This is an example pattern; use the actual URL shown by GitHub.

Every local page, photo, stylesheet and script uses relative paths. The site can therefore run under a repository subfolder without changing its paths.

### Updating the site from VS Code later

If your repository is already cloned onto your computer:

1. Open that repository folder in VS Code.
2. Copy these website files into its top level, keeping the `assets` folder intact.
3. Edit and preview your changes.
4. Open **Source Control**, review the changed files, enter a commit message, commit, then push/sync to GitHub.
5. GitHub Pages republishes changes pushed to the configured publishing branch.

Use your actual repository URL when cloning. No repository URL or account is hard-coded in these website files.

Official GitHub guides, checked for this project:

- [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [Configuring a publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## Files to edit

| File | Contents |
| --- | --- |
| `index.html` | Home, branding, mission, vision and commitment |
| `about.html` | Studio story, Essential/Advanced/Signature packages and Selected Works |
| `team.html` | Four team members, biographies and original studio video |
| `faqs.html` | Testimonials, seven FAQs and additional contact information |
| `contact.html` | Original address, phone numbers, email, social links, Bible verse and added enquiry draft form |
| `commercial.html` | Four commercial project names, addresses and original images |
| `residential.html` | Four residential project names, addresses and original images |
| `interiors.html` | Four interior project names, addresses and original images |
| `styles.css` | Shared Architrexx-derived styling plus Artizyn page layouts |
| `script.js` | Mobile menu, FAQs, image viewer, enquiry draft and chatbot panel |
| `assets/` | Original images and video saved from the current Canva website |
| `source-content.json` | Captured source text for comparing the rebuilt content |
| `CONTENT-CHECK.txt` | Results of the source-to-page text checks |

You can edit the HTML directly. Company content is present in each page's HTML, rather than being loaded from a database. The same header and footer appear on every page, so update each HTML file if you change shared navigation or footer text.

## How the websites were combined

- **Content and identity:** the linked Artizyn website is the source of truth.
- **Design and behaviour:** the first Architrexx code provides the blue gradients, glass-style cards, responsive layout, mobile menu, FAQ interaction and enquiry draft workflow.
- Original wording, spelling, team titles, testimonials, addresses, phone formatting and external social destinations are retained. Only layout-created whitespace/line breaks and duplicated responsive copies have been normalised.
- The original selected-work pages now use working local `.html` links. Get started leads to Contact, and package links preselect the requested package.
- Each project image opens in an enlarged viewer with that project's original name and address. Close it with the button, Escape, or the area outside the dialog.
- Canva's own hosting controls, animation time counters and platform policy overlays are not company content and are not reproduced. The company copyright text is retained.

Source: [Artizyn's current Canva website](https://shark-hxp7ny.my.canva.site/artizyn/).

## Existing Artizyn assistant

**Ask Artizyn** opens the original public Jotform assistant already embedded on the Canva home page. The assistant loads only when opened and has a link to open it separately if an embedded view is unavailable. It continues to depend on Jotform, the assistant owner's settings, and any service limits. No chat message was submitted while preparing or checking this website.

## Enquiry form

The contact form is adapted from the first Architrexx version and addressed to the **existing Artizyn email from your Canva site**: `artizyn.1254@gmail.com`.

It validates the fields and prepares a draft. **Open email app** opens a prefilled email for the visitor to review and send. It does not automatically send email or claim delivery. Visitors can also copy or download the draft. Nothing is stored by this website in local storage or a database. The page clearly describes this behaviour.

GitHub Pages does not run server-side form processing. Automatic form delivery would need a separate form service or backend. For a very long draft, use Copy or Download if an email app cannot handle the full mailto link.

## Common fixes

- **404 after publishing:** verify that `index.html` is at the root of the selected branch, and that Pages uses that branch with `/(root)`.
- **Images missing:** upload the complete `assets` folder. Keep filename spelling and upper/lowercase unchanged.
- **Changes not visible:** check the repository's Actions/deployment status and refresh after publishing finishes.
- **Email app does not open:** configure an email app on the computer, or use Copy draft/Download and send the draft manually.
- **Chatbot does not load:** it requires internet access and the original Jotform assistant to remain available. Use its new-tab link or the company's existing email.

## Local verification

The project is checked for page links, local assets, JavaScript syntax, source text preservation, and desktop/mobile behaviour. The included media is below GitHub's usual individual browser-upload size limit. A live GitHub deployment can only be verified after the project is uploaded to your repository and Pages is enabled.
