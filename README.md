# KDE Plasma Enhanced Panel 🚀

A highly customized and performance-optimized KDE Plasma panel with modern animations and visual enhancements.

![KDE Plasma](https://img.shields.io/badge/KDE-Plasma-1d99f3?style=for-the-badge&logo=kde&logoColor=white)
![QML](https://img.shields.io/badge/QML-Qt-41cd52?style=for-the-badge&logo=qt&logoColor=white)
![License](https://img.shields.io/badge/License-GPL--2.0-blue?style=for-the-badge)

## ✨ Features

This enhanced panel brings a premium desktop experience with the following improvements:

### 🎨 Visual Enhancements
- **Hover Rectangle Effects** - Smooth, elegant hover animations for panel items
- **App Icon Animations** - Beautiful open/close animations when launching or closing applications
- **Premium Aesthetics** - Refined visual design with modern styling
- **Improved Layout** - Better spacing and alignment for a cleaner look

### ⚡ Performance Improvements
- **Optimized Rendering** - Significantly faster panel performance
- **Reduced Resource Usage** - More efficient memory and CPU utilization
- **Smooth Animations** - Hardware-accelerated animations without lag

## 📁 Project Structure

```
.
├── configoverlay.qml    # Configuration overlay component
├── layoutmanager.js     # Layout management logic and utilities
└── main.qml            # Main panel component with core functionality
```

## 🔧 Installation

### Prerequisites
- KDE Plasma 5.x or 6.x
- Qt 5.15+ or Qt 6.x
- KDE Frameworks

### Installation Steps

1. **Backup your current panel configuration:**
   ```bash
   mkdir -p ~/.config/plasma-org.kde.plasma.desktop-appletsrc.backup
   cp ~/.config/plasma-org.kde.plasma.desktop-appletsrc ~/.config/plasma-org.kde.plasma.desktop-appletsrc.backup/
   ```

2. **Clone this repository:**
   ```bash
   git clone https://github.com/Vidithsoni01/kde-plasma-enhanced-panel.git
   cd kde-plasma-enhanced-panel
   ```

3. **Install the panel files:**
   ```bash
   # Copy files to the appropriate Plasma directory
   # For Plasma 5:
   cp *.qml ~/.local/share/plasma/plasmoids/org.kde.plasma.taskmanager/contents/ui/
   cp *.js ~/.local/share/plasma/plasmoids/org.kde.plasma.taskmanager/contents/code/
   
   # For Plasma 6:
   cp *.qml ~/.local/share/plasma/plasmoids/org.kde.plasma.taskmanager/contents/ui/
   cp *.js ~/.local/share/plasma/plasmoids/org.kde.plasma.taskmanager/contents/code/
   ```

4. **Restart Plasma:**
   ```bash
   kquitapp5 plasmashell && kstart5 plasmashell
   # Or for Plasma 6:
   kquitapp6 plasmashell && kstart plasmashell
   ```

## 🎥 Demo

*Add screenshots or GIFs here showing the hover effects, animations, and overall improvements*

## 📝 Customization

### Adjusting Animation Speed

Edit `main.qml` to modify animation durations:

```qml
// Find animation blocks and adjust duration values
NumberAnimation {
    duration: 200  // Modify this value (in milliseconds)
}
```

### Changing Hover Effects

In `configoverlay.qml`, you can customize the hover rectangle appearance:

```qml
// Customize hover rectangle properties
Rectangle {
    color: "your-color"
    opacity: 0.3
    radius: 4
}
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🐛 Known Issues

- None currently reported. If you find any bugs, please [open an issue](https://github.com/Vidithsoni01/kde-plasma-enhanced-panel/issues).

## 📋 TODO

- [ ] Add configuration GUI for easy customization
- [ ] Support for custom animation easing curves
- [ ] Additional theme variants
- [ ] Multi-monitor optimization
- [ ] More granular performance tuning options

## 🙏 Acknowledgments

- KDE Plasma Team for the amazing desktop environment
- The KDE community for inspiration and support

## 📄 License

This project is licensed under the GPL-2.0 License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Vidith Soni**

- GitHub: [@Vidithsoni01](https://github.com/Vidithsoni01)

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐ on GitHub!

---

<p align="center">Made with ❤️ for the KDE community</p>
