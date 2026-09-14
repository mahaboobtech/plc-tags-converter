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

### 2. PI Studio → Control Expert (`Live & Ready`)
- Converts Inovance PI Studio & WECON HMI Modbus tags (`0x`, `4x`, `4x.y`) back into EcoStruxure Control Expert PLC variables (`%M`, `%MW`, `%MWx.y`).
- **Reverse Address Mapping**:
  - `43000` (Word) $\rightarrow$ `%MW3000` (`INT` or `REAL`)
  - `4100.3` (Bit in Word) $\rightarrow$ `%MW100.3` (`EBOOL`)
  - `0100` (Coil Bit) $\rightarrow$ `%M100` (`EBOOL`)
- **Direct `.XSY` XML Export**: Generates Schneider Control Expert compatible `.XSY` files ready for 1-click import into Control Expert.

### 3. Plant SCADA → Control Expert (`Live & Ready`)
- **Direct Variable Database Parsing**: Supports drag & drop upload of AVEVA Plant SCADA / Citect SCADA `VARIABLE.CSV` files.
- **Modbus %MW / %M Filter**: Automatically extracts located Modbus tags (`%MW***`, `%MW***.bit`, `%M***`) and ignores unlocated SCADA internal tags.
- **Data Type Mapping**:
  - `UINT` $\rightarrow$ `UINT`
  - `WORD` $\rightarrow$ `WORD`
  - `INT` $\rightarrow$ `INT`
  - `REAL` / `FLOAT` $\rightarrow$ `REAL`
  - `DIGITAL` / `BOOL` / `%M` / `%MW.bit` $\rightarrow$ `EBOOL`
- **Direct `.XSY` XML Export**: Generates EcoStruxure Control Expert Variables Exchange `.XSY` XML files for instant 1-click import into Schneider Control Expert.

### 4. Control Expert → Plant SCADA (`Live & Ready`)
- **Direct `.XSY` File Parsing**: Upload raw `.xsy` variable export files from EcoStruxure Control Expert directly into the browser.
- **Reverse Data Type Mapping**:
  - `INT` $\rightarrow$ `INT`
  - `UINT` $\rightarrow$ `UINT`
  - `WORD` $\rightarrow$ `WORD`
  - `REAL` $\rightarrow$ `REAL`
  - `EBOOL` (with `%M***` or `%MW***.bit`) $\rightarrow$ `DIGITAL`
- **Modbus Sequential Address Sorting**: Automatically sorts exported tags sequentially (`%M0`...`%M100`, `%MW0`...`%MW500`).
- **32-Column `VARIABLE.CSV` Export**: Generates full 32-column AVEVA Plant SCADA / Citect `VARIABLE.CSV` with formatted quotes and headers ready for SCADA DBF/CSV database import.

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
