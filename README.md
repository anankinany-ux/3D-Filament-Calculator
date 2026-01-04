# 3D Printing Filament Cost Calculator

A comprehensive web-based calculator for 3D printing enthusiasts to calculate filament costs, manage filament profiles, and price their prints accurately.

![Calculator Preview](https://img.shields.io/badge/Status-Ready-green)
![License](https://img.shields.io/badge/License-MIT-blue)

## Features

✨ **Multi-Currency Support**: Calculate costs in over 20 currencies including USD, EUR, GBP, ILS, JPY, and more

📊 **Comprehensive Cost Calculations**: 
- Material cost based on filament weight
- Selling price calculations by weight and/or print time
- Support for custom pricing per gram and per minute

🎨 **Filament Profile Management**:
- Save multiple filament profiles
- Custom naming for easy identification
- Track filament type, manufacturer, color, diameter, density, and pricing
- Edit and delete saved profiles
- Visual color previews

🌐 **Bilingual Interface**:
- English and Hebrew (עברית) language support
- RTL (Right-to-Left) support for Hebrew
- Persistent language preference

📱 **Responsive Design**:
- Mobile-friendly interface
- Works on desktop, tablet, and mobile devices
- Touch-optimized controls

💾 **Local Storage**:
- All data saved locally in your browser
- No server required - works completely offline
- Your filament profiles and preferences persist across sessions

## Usage

### Basic Calculation

1. **Enter Model Weight**: Input the weight of your 3D printed model in grams
2. **Enter Print Time**: Specify the print time in hours and minutes
3. **Select Filament**: Choose a saved filament profile or enter filament details manually
4. **Calculate**: Click "Calculate Cost" to see detailed cost breakdown

### Managing Filament Profiles

1. **Add New Filament**: Click the "+ Add Filament" button
2. **Enter Details**:
   - Custom name (optional)
   - Filament type (PLA, PETG, ABS, etc.)
   - Manufacturer
   - Color
   - Diameter (typically 1.75mm or 2.85mm)
   - Price per kilogram
   - Density (g/cm³)
   - Selling price per gram (optional)
   - Selling price per minute (optional)
3. **Save Profile**: Click "Save Filament Profile"
4. **Edit/Delete**: Use the edit (✎) or delete (×) buttons on saved profiles

### Currency Selection

- Use the currency selector in the top-left corner
- Choose from 20+ supported currencies
- All prices will automatically update to display in the selected currency
- Your currency preference is saved for future sessions

### Language Selection

- Switch between English and Hebrew using the language buttons in the header
- The interface will update immediately, including RTL layout for Hebrew

## Supported Filament Types

- PLA
- PLA+
- PETG
- PET
- ABS
- TPU
- ASA
- PC (Polycarbonate)
- Nylon
- Other (custom)

## Supported Currencies

- **₪ ILS** - Israeli Shekel
- **$ USD** - US Dollar
- **€ EUR** - Euro
- **£ GBP** - British Pound
- **¥ JPY** - Japanese Yen
- **C$ CAD** - Canadian Dollar
- **A$ AUD** - Australian Dollar
- **CHF** - Swiss Franc
- **¥ CNY** - Chinese Yuan
- **₹ INR** - Indian Rupee
- **R$ BRL** - Brazilian Real
- **₩ KRW** - South Korean Won
- **$ MXN** - Mexican Peso
- **₽ RUB** - Russian Ruble
- **R ZAR** - South African Rand
- **kr SEK** - Swedish Krona
- **kr NOK** - Norwegian Krone
- **kr DKK** - Danish Krone
- **zł PLN** - Polish Złoty
- **₺ TRY** - Turkish Lira

## Technical Details

### How It Works

The calculator uses the following formulas:

1. **Filament Length Calculation**:
   ```
   Volume (cm³) = Weight (g) / Density (g/cm³)
   Volume (mm³) = Volume (cm³) × 1000
   Cross-section Area (mm²) = π × (Diameter/2)²
   Length (mm) = Volume (mm³) / Cross-section Area (mm²)
   Length (m) = Length (mm) / 1000
   ```

2. **Material Cost**:
   ```
   Material Cost = Weight (g) × Price per Gram
   ```

3. **Selling Price**:
   ```
   By Weight = Weight (g) × Price per Gram
   By Time = Print Time (min) × Price per Minute
   Total = By Weight + By Time (if both are set)
   ```

### Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Technologies Used

- Pure HTML5, CSS3, and JavaScript
- No frameworks or dependencies required
- LocalStorage API for data persistence
- Responsive CSS Grid and Flexbox layouts

## Installation

No installation required! This is a single HTML file that runs entirely in your browser.

1. Download `filament-calculator.html`
2. Open it in any modern web browser
3. Start calculating!

### For GitHub Pages Deployment

1. Fork or clone this repository
2. Enable GitHub Pages in repository settings
3. Select the branch containing `filament-calculator.html`
4. Your calculator will be live at `https://yourusername.github.io/repository-name/filament-calculator.html`

## File Structure

```
filament-calculator/
├── filament-calculator.html  # Main application file (all-in-one)
├── README.md                 # This file
├── LICENSE                   # MIT License
└── .gitignore               # Git ignore rules
```

## Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Created for 3D printing enthusiasts who want to accurately calculate and price their prints.

## Support

If you find this calculator useful, consider:
- ⭐ Starring this repository
- 🐛 Reporting bugs
- 💡 Suggesting improvements
- 📢 Sharing with other 3D printing enthusiasts

## Changelog

### Version 1.0
- Initial release
- Multi-currency support
- Filament profile management
- Bilingual interface (English/Hebrew)
- Responsive design
- Local storage persistence

---

**Happy Printing! 🖨️✨**

