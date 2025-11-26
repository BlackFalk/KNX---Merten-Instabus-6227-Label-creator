# Merten Instabus 6227 Label Editor

A web-based editor for creating custom labels for Merten Instabus 6227 multifunction switches.

Created with claude.ai

![Merten 6227 Label Editor](screenshot.png)

## 📋 Overview

The Merten Instabus 6227 is a KNX multifunction switch with 8 programmable buttons (4 left, 4 right). This editor allows you to create professional labeling stickers for the center recess of the switch.

## ✨ Features

- 🏷️ **Multi-Label Editor**: Create multiple labels simultaneously
- 🎨 **33 Predefined Symbols**: Light bulb, fan, lock, door, and many more
- ✏️ **Fully Editable**: All room names and symbols individually customizable
- 📐 **Correct Dimensions**: Exactly 32 mm × 47 mm (3.2 cm × 4.7 cm)
- 🖨️ **Print Ready**: Optimized for self-adhesive label sheets
- 👁️ **Live Preview**: Changes are displayed immediately
- ☑️ **Enable/Disable Rows**: For partially configured switches
- 🌐 **Works Offline**: No internet connection required

## 🚀 Installation

1. Clone or download the repository:
```bash
git clone https://github.com/YOUR-USERNAME/merten-6227-label-editor.git
cd merten-6227-label-editor
```

2. Open the `merten_label_editor.html` file in your browser
   - Simply double-click or
   - Open with a local web server

## 📁 Project Structure

```
merten-6227-label-editor/
├── merten_label_editor.html    # Main editor file
├── Symbols/                     # Folder with all symbol icons
│   ├── symbol1.png             # Power symbol
│   ├── symbol15.png            # Light bulb
│   ├── symbol20.png            # Fan
│   └── ...                     # 33 symbols total
└── README.md                   # This file
```

## 🎯 Usage

### Step 1: Open Editor
Open `merten_label_editor.html` in a modern web browser (Chrome, Firefox, Edge, Safari).

### Step 2: Create Labels
1. **Add New Label**: Click on "➕ Add New Label"
2. **Assign Name**: Give the label a name (e.g., "Living Room", "1st Floor")
3. **Configure Rows**:
   - Enter room names (e.g., "Bathroom", "Hallway", "Kitchen")
   - Select appropriate symbols from the dropdown
   - Disable unused rows with the checkbox
4. **Check Preview**: Changes are automatically displayed in the preview

### Step 3: Print
1. Click on "🖨️ Print All Labels"
2. In the print dialog:
   - Select **"Actual Size"** or **"100% Scale"**
   - Disable **"Fit to Page"**
3. Print on self-adhesive label sheets or regular paper
4. Cut along the dashed lines

## 📐 Technical Specifications

- **Label Dimensions**: 32 mm × 47 mm (3.2 cm × 4.7 cm)
- **Rows per Label**: 4 (each 11.75 mm high)
- **Symbol Format**: PNG, optimized for 5-6 mm height
- **Font Size**: 2.5 mm for optimal readability
- **Layout**: ON - [Symbol] - OFF per row

## 🎨 Available Symbols

The editor includes 33 predefined symbols:

| Category | Symbols |
|-----------|---------|
| **Light** | Bulb, Sun, Moon |
| **Control** | Power, Plus, Minus, Arrows |
| **Devices** | Fan, Heater, Speaker, Monitor |
| **Security** | Lock, Key, Eye, Door |
| **Miscellaneous** | Bell, Clock, Music, Settings, House |

## 🛠️ Customization

### Adding Custom Symbols

1. Create PNG images with transparent background
2. Recommended size: 300x300 pixels
3. Save them in the `Symbols/` folder as `symbol34.png`, `symbol35.png`, etc.
4. Add new entries in the HTML code in the `symbols` array:

```javascript
const symbols = [
    // ... existing symbols
    { file: 'symbol34.png', name: '🆕 Your Symbol' }
];
```

## 🖨️ Printing Tips

### Recommended Materials
- **Self-adhesive Label Sheets**: White, matte or glossy
- **Paper Format**: A4
- **Printer**: Inkjet or Laser

### Print Settings
- **Quality**: Highest Quality / Photo Quality
- **Scale**: 100% / Actual Size
- **Orientation**: Portrait
- **Margins**: Default

### After Printing
1. Cut along the dashed lines
2. Test the fit on the switch
3. Clean the switch surface before applying
4. Apply the label centered

## 🔧 System Requirements

- **Browser**: Modern web browser with JavaScript support
  - Chrome 90+
  - Firefox 88+
  - Safari 14+
  - Edge 90+
- **Operating System**: Windows, macOS, Linux
- **Printer**: Any printer with A4 support

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

- 🐛 Report bugs
- 💡 Suggest new features
- 🎨 Add new symbols
- 📖 Improve documentation
- 🌍 Add translations

### Pull Requests
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/NewFeature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/NewFeature`)
5. Open a Pull Request

## 📧 Contact & Support

- **Issues**: Use GitHub Issues for bug reports and feature requests
- **Discussions**: GitHub Discussions for general questions

## ⚙️ Compatibility

Tested with:
- ✅ Merten Instabus 6227 Multifunction Switch
- ✅ Various browsers (Chrome, Firefox, Safari, Edge)
- ✅ Windows 10/11, macOS, Linux

## 📚 Further Links

- [Merten Product Page](https://www.merten.de)
- [KNX Standard](https://www.knx.org)
- [Instabus EIB/KNX](https://en.wikipedia.org/wiki/KNX_(standard))

## 👏 Acknowledgments

- Icons/Symbols: Custom creation or royalty-free sources
- Merten/Schneider Electric for developing the 6227 switch

## 📄 Changelog

### Version 1.0.0 (2024-11-26)
- ✨ Initial release
- 🏷️ Multi-label editor
- 🎨 33 predefined symbols
- 🖨️ Print function with correct dimensions
- ✏️ Fully editable labels

---

**Note**: This project is not officially affiliated with Merten or Schneider Electric.
