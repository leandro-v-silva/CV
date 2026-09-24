📄 Leandro Vieira Silva — CV

Welcome! This repository contains my personal resume (CV), written in LaTeX (AltaCV) and served through a lightweight landing page with a built-in language switcher — fully automated with GitHub Actions CI/CD.

🌐 Live Demo

👉 [leandro-v-silva.github.io/CV](https://leandro-v-silva.github.io/CV/)

✨ Features

- 🌍 Bilingual — switch between Portuguese 🇧🇷 and English 🇺🇸 with one click
- 📄 Embedded PDF viewer — preview the CV directly in the browser
- ⬇️ Download button — get the PDF in the selected language
- 🎨 Custom design based on the AltaCV template, with my own color scheme
- 🤖 Fully automated — edit the `.tex` files, push, and GitHub Actions compiles + deploys everything

🚀 Built With

- LaTeX — CV content & layout (AltaCV class)
- HTML5 / CSS3 — landing page
- JavaScript — language toggle & PDF download
- GitHub Actions — CI/CD pipeline
- GitHub Pages — hosting

🔄 CI/CD Workflow

The GitHub Actions workflow [`.github/workflows/build-cv.yml`](.github/workflows/build-cv.yml) runs automatically on every push that changes files in `tex/`:

1. 📥 Checks out the repository
2. 🔨 Compiles `resume_en.tex` and `resume_pt.tex` to PDF
3. 📦 Moves the compiled PDFs to the repo root
4. 🤖 Auto-commits the updated PDFs with the message "chore: auto-build resume PDFs from LaTeX source"

📁 Project Structure

```
📦 CV
├── index.html                     # Landing page with language toggle (PT/EN)
├── resume_en.pdf                  # English CV (auto-compiled)
├── resume_pt.pdf                  # Portuguese CV (auto-compiled)
├── tex/
│   ├── altacv.cls                 # AltaCV class file
│   ├── resume_en.tex              # English CV source
│   └── resume_pt.tex              # Portuguese CV source
├── .github/
│   └── workflows/
│       └── build-cv.yml           # CI/CD: auto-compile LaTeX → PDF
└── README.md / README.pt.md
```

🛠️ How to Update the CV

1. Clone the repository:
   
```bash
   git clone https://github.com/leandro-v-silva/CV.git
   ```

2. Edit `tex/resume_en.tex` and/or `tex/resume_pt.tex` with any text editor or Overleaf.
3. Commit and push:
   
```bash
   git add tex/
   git commit -m "update resume content"
   git push
   ```

4. ✅ Done! The GitHub Actions workflow automatically compiles the new PDFs and updates the live site.

📬 Contact

- 📧 Email: [leandro797.ls@gmail.com](mailto:leandro797.ls@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/leandro-vieira-silva-analytics](https://www.linkedin.com/in/leandro-vieira-silva-analytics)
- 🐙 GitHub: [github.com/leandro-v-silva](https://github.com/leandro-v-silva)
- 📍 São Paulo, Brazil

---

⭐ If you like this project, feel free to give it a star!

Last updated: September 2026
