# PLC Tags Converter Suite ⚡

A modern, web-based suite of industrial automation tag conversion tools for PLC programmers and SCADA/HMI engineers. Easily transform variable databases between **Schneider Electric Control Expert**, **AVEVA Plant SCADA (Citect)**, and **Inovance PI Studio (WECON HMI)** formats.

---

## 🌐 Live Web App (GitHub Pages)
👉 **[https://mahaboobtech.github.io/plc-tags-converter/](https://mahaboobtech.github.io/plc-tags-converter/)**

---

## 🚀 Converter Modules Roadmap

### 1. Control Expert → PI Studio (`Live & Ready`)
- Direct **`.XSY`** file support: Upload raw `.xsy` variable export files from EcoStruxure Control Expert directly into the browser (no Excel macro tool needed!).
- **Address Mapping**:
  - `%MW100` $\rightarrow$ `W` / `4100`
  - `%MW100.3` $\rightarrow$ `X` / `4100.3`
  - `%M100` $\rightarrow$ `X` / `0100`
- **Modbus Sequential Sorting**: Automatically sorts converted tags by address order.
- **Direct PI Studio Export**: Generates `.xls` (BIFF8) files formatted with required `DSO_DX` sheet name and forced text encoding (`@`).

### 2. PI Studio → Control Expert (`Upcoming`)
- Converts Inovance PI Studio & WECON HMI Modbus tags (`0x`, `4x`) back into EcoStruxure Control Expert PLC variables (`%M`, `%MW`, `%MWx.y`).

### 3. Plant SCADA → Control Expert (`Upcoming`)
- Transform AVEVA Plant SCADA (formerly Citect SCADA) variable databases (`variable.dbf` / `.csv`) into EcoStruxure Control Expert PLC variable imports (`.XLS` / `.CSV`).

### 4. Control Expert → Plant SCADA (`Upcoming`)
- Convert EcoStruxure Control Expert PLC variables (`%M`, `%MW`, unlocated tags) into AVEVA Plant SCADA variable tag definitions.

---

## 🔒 Security & Privacy
- **100% In-Browser & Private**: All conversions run strictly inside your web browser. Zero files or tag data are uploaded to any external server.

---

## 👨‍💻 Developer & Branding
- **Official Website**: [mahaboobtech.in](https://mahaboobtech.in)
- **GitHub Repository**: [mahaboobtech/plc-tags-converter](https://github.com/mahaboobtech/plc-tags-converter)

---

## 📄 License & Copyright
© 2026 **mahaboobtech**. Licensed under the [MIT License](LICENSE).
