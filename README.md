# Minimalist Poetry Book Template
### A simple, clean LaTeX template for poetry collections.

I originally created this template to compile a friend's poetry into an eBook. I wanted something that was elegant, easy to edit, and simple to repurpose for print or digital distribution.

**Tested on Overleaf.**

I am sharing this so that anyone can publish their own poetry in a professional, minimalist design without needing to be a coding expert.

## Features

- **A5 Format:** Perfect for pocket books or digital reading.
- **Minimalist Design:** clean typography using Palatino and a soft gray color scheme.
- **Automated Table of Contents:** Automatically updates when you add new poems.
- **Beginner Friendly:** The code is heavily commented so you know exactly where to type.

---

## How to Use (No Git/Coding Knowledge Required)

1. Go to [Overleaf.com](https://www.overleaf.com/) and create a free account.
2. Click **"New Project"** -> **"Blank Project"**.
3. Open the `main.tex` file (it is created automatically).
4. Delete **everything** currently inside that file.
5. **Copy and Paste** the standardized code from `poetry.tex` (in this repository) into the editor.
6. Click the **Recompile** button (green button) to see your book.

---

## *Note: Gemini 3 Pro was used to standardize the code structure and improve readability. with the following prompt: "can you standardize this code and make helpful comments for starters"

---
## Customization Guide

You only need to change the text in specific places. The file is organized with clear headers like `% --- SECTION NAME ---`.

### 1. The Cover
Scroll down until you see `% --- TITLE PAGE (CAPA) ---`.
- Replace `Nome do Autor` with your name.
- Replace `TÍTULO`, `DA`, `OBRA` with your title words.
- Replace `Fortaleza, 2026` with your city and year.

### 2. Credits / Copyright
Look for `% --- TECHNICAL PAGE (FICHA TÉCNICA) ---`.
- Change `Autora: Taz`, `Ano`, and `ISBN` to your details.

### 3. Adding Your Poems
Scroll to `% --- POEMS START HERE ---`.

To add a new poem, copy and paste the block below.

**Important:**
- Use `\\` at the end of a line to break it.
- Use `\vspace{0.5cm}` to create a gap between stanzas.

#### Code Snippet for a New Page Poem:
```latex
\newpage                % Starts a new page
\poema{Title of Poem}   % Your title -> automatically goes to the Table of Contents

\vspace*{\fill}         % Centers the poem vertically 

\begin{verse}
    This is the first line \\      % Use double backslash to break line
    This is the second line \\
    
    \vspace{0.5cm}      % Adds space between stanzas
    
    This is a new stanza \\
    lines continue here
\end{verse}

\vspace*{\fill}         % Centers the poem vertically
