# PathTransfer

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Photoshop](https://img.shields.io/badge/Photoshop-CS6+-ff00ff)
![Status](https://img.shields.io/badge/status-active-success)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)

Professional JSX/ExtendScript automation script for Adobe Photoshop. Engineered for workflow automation by transferring clipping paths between files based on filename matching, eliminating repetitive manual path recreation across batches.

---

## Overview

PathTransfer automates the process of transferring clipping paths from one file to another using filename matching. Perfect for batch workflows where paths need to be replicated across multiple file formats or versions, significantly reducing manual path recreation time.

### Capabilities

- Transfer clipping paths between file formats by filename
- Batch path transfer automation
- Production-ready implementation
- Non-destructive operations
- Cross-platform support (macOS, Windows)
- Extensive version compatibility (CS6+)

---

## Installation

### macOS

```bash
git clone https://github.com/TheMaestr-o/path-transfer.git
cp PathTransfer.jsx ~/Library/Application\ Support/Adobe/Adobe\ Photoshop\ [VERSION]/Presets/Scripts/
```

**Version-specific paths:**
- Photoshop 2025: `~/Library/Application Support/Adobe/Adobe Photoshop 2025/Presets/Scripts/`
- Photoshop 2024: `~/Library/Application Support/Adobe/Adobe Photoshop 2024/Presets/Scripts/`
- Photoshop 2023: `~/Library/Application Support/Adobe/Adobe Photoshop 2023/Presets/Scripts/`
- Photoshop CC 2020: `~/Library/Application Support/Adobe/Adobe Photoshop 2020/Presets/Scripts/`

### Windows

```bash
git clone https://github.com/TheMaestr-o/path-transfer.git
copy PathTransfer.jsx "C:\Program Files\Adobe\Adobe Photoshop [VERSION]\Presets\Scripts\"
```

**Version-specific paths:**
- Photoshop 2025: `C:\Program Files\Adobe\Adobe Photoshop 2025\Presets\Scripts\`
- Photoshop 2024: `C:\Program Files\Adobe\Adobe Photoshop 2024\Presets\Scripts\`
- Photoshop 2023: `C:\Program Files\Adobe\Adobe Photoshop 2023\Presets\Scripts\`

### Quick Setup

1. Download `PathTransfer.jsx`
2. Open Photoshop
3. File → Scripts → Browse
4. Select script
5. Execute

---

## Usage

### Method 1: Photoshop Menu

```
File → Scripts → Other Scripts → PathTransfer
```

### Method 2: Scripts Panel

1. Window → Scripts
2. Locate "PathTransfer"
3. Double-click

### Method 3: ExtendScript Console

```javascript
#include "/path/to/PathTransfer.jsx"
main();
```

---

## Workflow

### Typical Scenario

1. Source file (e.g., `product_001.psd`) contains clipping path
2. Target file (e.g., `product_001.tif`) needs same path
3. Execute PathTransfer script
4. Script matches filenames and transfers path
5. Target file receives path automatically

### Batch Processing

- Process multiple file pairs simultaneously
- Filenames must match (excluding extension)
- Place source files in designated folder
- Run script to transfer paths batch-wide

---

## Technical Specifications

### System Requirements

| Component | Specification |
|-----------|---------------|
| Operating System | macOS 10.11+ / Windows 10+ |
| Photoshop | CS6+ |
| Runtime | ExtendScript (included with Photoshop) |
| Dependencies | None |

### Compatibility Matrix

| Photoshop Version | Support |
|-------------------|---------|
| CS6 | ✓ |
| CC 2015 | ✓ |
| CC 2017 | ✓ |
| CC 2018 | ✓ |
| CC 2019 | ✓ |
| CC 2020 | ✓ |
| CC 2021 | ✓ |
| CC 2022 | ✓ |
| CC 2023 | ✓ |
| CC 2024 | ✓ |
| CC 2025 | ✓ |

---

## Supported File Formats

- PSD (Photoshop Document)
- TIF/TIFF (Tagged Image File)
- PNG (with path support)
- PDF (when Photoshop path enabled)

---

## FAQ

**Q: Script not appearing in Photoshop menu**

A: Verify installation path matches your Photoshop version. Restart Photoshop. Confirm .jsx file extension is correct.

**Q: Filename matching fails**

A: Ensure filenames match exactly (excluding extension). Example: `product_001.psd` matches `product_001.tif`.

**Q: Path not transferred**

A: Source file must contain clipping path. Verify path exists before running script. Check file access permissions.

**Q: Different file formats**

A: Script supports transfer between different formats. Format conversion handled automatically.

**Q: Batch processing multiple files**

A: Place source and target files in same folder. Filenames must match. Execute script to process all pairs.

**Q: Performance optimization**

A: Processing speed depends on path complexity. Large path libraries process quickly. Close unnecessary applications.

---

## Licensing

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Support & Contact

For questions, feedback, or collaboration:

[![Email](https://img.shields.io/badge/Email-gssdarm%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:gssdarm@gmail.com)
[![Telegram](https://img.shields.io/badge/Telegram-%40ohnedan-0088cc?style=flat-square&logo=telegram&logoColor=white)](https://t.me/ohnedan)
[![GitHub](https://img.shields.io/badge/GitHub-TheMaestr--o-black?style=flat-square&logo=github&logoColor=white)](https://github.com/TheMaestr-o)

---

Part of the [Photoshop-Scripts](https://github.com/TheMaestr-o/Photoshop-Scripts) collection.

Last updated: June 2026
