# Control Expert → PI Studio Converter

A modern, web-based converter tool to transform Schneider Electric **Control Expert** PLC variables (Excel/Export format) into **WECON PI Studio HMI** compatible tag format (`DSO_DX`).

---

## 🌐 Live Web App (GitHub Pages)
👉 **[https://mahaboobtech.github.io/controlexpert-to-pi-studio-tags-convertor/](https://mahaboobtech.github.io/controlexpert-to-pi-studio-tags-convertor/)**

---

## ⚡ Features & Address Rules
- **100% Client-Side & Private**: Conversion runs entirely inside your browser. No files are uploaded to any server.
- **Automatic Address Mapping**:
  - `%MW100` $\rightarrow$ `W` / `4100`
  - `%MW100.3` $\rightarrow$ `X` / `4100.3`
  - `%M100` $\rightarrow$ `X` / `0100`
- **Modbus Sorting**: Automatically sorts converted tags by Modbus address order.
- **Direct PI Studio Export**: Generates `.xls` file formatted with required `DSO_DX` sheet name and forced text encoding (`@`).

---

## 👨‍💻 Developer & Branding
- **Official Website**: [mahaboobtech.in](https://mahaboobtech.in)
- **GitHub Profile**: [@mahaboobtech](https://github.com/mahaboobtech)

---

## 📄 License & Copyright
© 2026 **mahaboobtech**. Licensed under the [MIT License](LICENSE).
