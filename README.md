# AssID-Stripper

[![Live Utility](https://img.shields.io/badge/Live_App-GitHub_Pages-16a34a?style=flat-square&logo=github)](https://blainekyle.github.io/AssID-Stripper/)

**Client-side CSV header cleaner that strips trailing 7-digit LMS assignment IDs (`(1234567)`) from gradebook exports.**

Launch in browser: **[blainekyle.github.io/AssID-Stripper](https://blainekyle.github.io/AssID-Stripper/)**

---

## Overview

Gradebook CSV exports (such as Canvas LMS) append 7-digit assignment identifiers in parentheses to the end of column headers — for example, `Midterm Exam (1234567)` — which can break downstream spreadsheet formulas, mail merges, or reporting imports.

**AssID-Stripper** removes trailing ` (#######)` suffixes from CSV column headers in a single click while leaving all row data untouched.

## Features

- **100% Browser-Local Privacy**: Uses the HTML5 `FileReader` and `Blob` APIs directly in your browser tab — student or gradebook CSV files are never uploaded to any server.
- **Non-Destructive Export**: Automatically generates a clean `<filename>_AssIDStripped.csv` download while preserving your original file.
- **Zero Setup**: Single standalone web page hosted on GitHub Pages (or open `index.html` locally offline).