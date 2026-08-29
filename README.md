# controlexpert-to-pi-studio-tags-convertor

A web-based converter tool to transform Schneider Electric **Control Expert** PLC variables (Excel/Export format) into **PI Studio** (Wintek / Weinview / PI Studio HMI) compatible tag format.

## 🚀 Live Web App (GitHub Pages)
👉 **[https://mahaboobtech.github.io/controlexpert-to-pi-studio-tags-convertor/](https://mahaboobtech.github.io/controlexpert-to-pi-studio-tags-convertor/)**

---

## ✨ Features
- **Client-Side Security**: All conversions take place locally in your browser. No files are uploaded to any server.
- **Excel Input (.xlsx / .xls)**: Upload your Control Expert export file easily via drag-and-drop or file picker.
- **Automatic Address Mapping**:
  - `%MW100` $\rightarrow$ `40100` (`4` type)
  - `%M100` $\rightarrow$ `00100` (`X` type)
- **PI Studio Ready**: Generates a `.xls` file with the exact sheet format (`DSO_DX`) required by PI Studio.

---

## ⚙️ Enabling GitHub Pages
1. Go to your repository on GitHub: `https://github.com/mahaboobtech/controlexpert-to-pi-studio-tags-convertor`
2. Open **Settings** $\rightarrow$ **Pages** (under Code and automation).
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`
   - **Branch**: Select `main` and `/ (root)`
4. Click **Save**.
