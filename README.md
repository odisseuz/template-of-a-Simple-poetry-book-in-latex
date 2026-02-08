# Minimalist Poetry Book Template
### A simple LaTeX template for poetry collections

I originally created this template to compile a friend's poetry into a eBook. I wanted something that was easy to edit and repurpose. 

Tested on Overleaf.

I am sharing this so that anyone can publish their own poetry in a minimalist design.

*Note: Gemini 3 Pro was used to standardize the code structure and improve readability.*

## Features

- A5 Format
- Minimalist Design
- Automated Table of Contents (Uploads when you write the poetry inside the code)
- Beginner Friendly — The main goal of this small project
---
## How to Use (for people who are not used with gitand github)
1.  Go to [Overleaf.com](https://www.overleaf.com/) and create a free account.
2.  Click **"New Project"** -> **"Blank Project"**.
3.  Open the `main.tex` file (it's created automatically).
4.  Delete everything currently in that file.
5.  **Copy and Paste** the code from the `poetry.tex` file in this repository into the editor.
6.  Click the **Recompile** button (green button) to see your book.
---
You only need to change the text in **4 specific places**. The rest of the code handles the design for you.

### 1. Changing the Contents of the COver
Scroll down until you see `% Capa`.
- Replace `Nome do Autor` with your name.
- Replace `TÍTULO`, `DA`, `OBRA` with your title.
- Replace `Fortaleza, 2026` with your city and year.

### 2. Credits
Look for `% PÁGINA 2: FICHA TÉCNICA`.
- Change `Autora: Taz` and the `Ano` to your details.

### 3. Adding Your Poems
Scroll to `% --- INÍCIO DOS POEMAS ---`.

---
#### How to add a new poem:

This centers the poem vertically on the page.

```latex

\newpage                % Starts a new page
\poema{Title of Poem}   % Your title -> automatically goes to summary

\vspace*{\fill}         % Centers the poem vertically 
\begin{verse}
    This is the first line \\      % Use \\ to break the line
    This is the second line \\
    
    \vspace{0.5cm}      % Adds vertical space
    
    This is a new stanza \\
    lines continue here
\end{verse}
\vspace*{\fill}         % Centers the poem vertically

%or you can do not use a \newpage and separate using \vspace{} for multiple poems on the same page


with the new code, can you atualize the readme
