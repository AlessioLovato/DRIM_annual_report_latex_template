DRIM PhD Annual Report – LaTeX Template
=======================================

This repository contains a LaTeX template for the annual report of the
[**DRIM PhD programme**](https://drim.i-rim.it/en/) (Robotics and Intelligent Machines), designed to
closely reproduce the structure and visual style of the official Word
document provided by the course office.

The template is intended for PhD students who prefer to prepare their
report in LaTeX while still delivering a PDF that matches the expected
layout and headings.

> [!WARNING]
> This document is **`UNOFFICIAL`**

## 1. Repository contents

- `main.tex` – main LaTeX source for the annual report.
- `figures/logo.png` – official DRIM logo.
- `LICENSE` – Apache 2.0 license for this template.

You normally only need to edit `main.tex` and add figures.


## 2. Requirements

The template is compatible with a standard, up‑to‑date LaTeX installation.

Recommended environment:

- **Engine**: `pdflatex`
- **Distribution**: TeX Live 2023 or later (or equivalent MiKTeX)

Packages used (loaded in `main.tex`):

- Layout and spacing: `geometry`, `setspace`, `titlesec`, `enumitem`
- Tables and alignment: `array`, `tabularx`, `ragged2e`
- Header / footer: `fancyhdr`
- Links and metadata: `hyperref`
- Graphics: `graphicx`
- Fonts: `mathptmx`, `fontenc` with `T1`
- Utilities: `xparse` (for the subsection macro)


## 3. Compiling the document

You can work with this template either on [**Overleaf**](https://www.overleaf.com/) or **locally with `pdflatex`**.

### 3.1 Using Overleaf (recommended)

1. Create a new Overleaf project (blank or “Upload project”).
2. Upload `main.tex`, the `figures/` folder (including `logo.png`), and
	optionally `LICENSE`.
3. Make sure the compiler is set to **pdfLaTeX**.
4. Click **Recompile** to generate `main.pdf`.

Overleaf will automatically run LaTeX enough times to resolve cross‑
references and the table of contents.

### 3.2 Local compilation with `pdflatex`

From the repository root:

```bash
pdflatex main.tex
pdflatex main.tex   # run twice for references / TOC if needed
```

This will produce `main.pdf`, which you can submit as your DRIM annual
report.


## 4. Overall layout and style

Key layout decisions have been chosen to imitate the official DOCX:

- **Paper size**: A4, margins `top=2.5cm`, `bottom=2cm`, `left=2cm`, `right=2cm`.
- **Font**: Times‑like font via `mathptmx`, with `T1` encoding.
- **Line spacing**: set so that text density is similar to the official form.
- **Page style**: page number centered in the footer, no header rule.
- **Heading style**:
	- `\section` headings are numbered (`1.`, `2.`, …) and formatted in a
		Word‑Heading‑3–like style (bold, small caps, slightly larger font).
	- `\subsection` headings are numbered (`1.1`, `1.2`, …) and bolded
		via the custom macro (see below).
	- `\subsubsection*` is used for small titled blocks (e.g. tables),
		without numbering and without appearing in the table of contents.


## 5. How to edit the template

1. **Fill in the header fields**
	 - Complete `Student`, `Cycle`, `Tutor(s)`, `Year`, `Contacts` lines
		 near the top of `main.tex`.

2. **Adjust the curriculum line**
	 - Add your curriculum name.

3. **Write your research activity**
	 - For each subsection under *Research Activity*, replace the
		 placeholder comment with your text.

4. **Populate the training and activity tables**
	 - For each table under *Training related to the PhD Program* and
		 *Other activities*, add as many rows as required.
	 - Keep the structure (columns and header row) unchanged to maintain
		 compatibility with the expected form.

5. **Signatures**
	 - Print the PDF and sign in the corresponding fields (PhD Student,
		 Tutor(s)).


## 6. Relation to the official DRIM documentation

The official rules and forms for the DRIM PhD programme are published
on the programme website:

- https://drim.i-rim.it/it/

This LaTeX template is **unofficial** and aims only to reproduce the
layout and information requested by the Word/DOCX annual‑report form.
If there is any discrepancy between this template and the official
documentation, the latter always prevails.


## 9. License

This template is released under the **Apache License 2.0**.

See `LICENSE` for the full license text and usage conditions.
