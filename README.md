# Community-Fflags

Fflags-storage powered by contributors and known users

---

## 📖 About

This repository is a centralized collection of FFlags (Feature Flags) contributed by the community. FFlags are configuration settings used to enable or disable features in Roblox games. This project allows multiple contributors to maintain FFlags organized by game and general use cases.

---

## 🚀 Quick Start - Contributor Tutorial

### How FFlags Are Organized

FFlags in this repository are stored in two ways:

1. **General FFlags** - Apply to all games (stored in the general file)
2. **Game-Specific FFlags** - Apply to a single game (stored in game folders)

---

## 📝 How to Contribute

### Adding General FFlags

For FFlags that work across multiple games:

1. Add your FFlags to the **general file** in JSON format
2. Follow the JSON requirements below
3. Add your name as a contributor at the bottom of the file

### Adding Game-Specific FFlags

For FFlags that apply to only one game:

1. Add your FFlags to the **appropriate game folder**
2. If the game folder doesn't exist, create one following the instructions below
3. Follow the JSON requirements below

---

## 📁 Creating a New Game Folder

To add FFlags for a game that doesn't have a folder yet:

1. **Create a new folder** with the game name
2. **Create a `place-id.ini` file** in the folder containing:
   - Only the Roblox Place ID (nothing else)
   ```
   12345678
   ```
3. **Add JSON files** in the same folder containing your FFlags
   - File naming convention: `fflags.json` or descriptive names like `gameplay.json`, `graphics.json`, etc.

---

## 📋 JSON File Requirements

### FFlags Format

All FFlags **must** be contained within curly braces `{}`. Any FFlags not following this format will be ignored or marked as unavailable.

✅ **Correct:**
```json
{
  "FFlagSampleFeature": true,
  "FFlagAnotherFeature": false,
  "DFFlagExampleSetting": "value"
}
// #your-contributor-name
```

❌ **Incorrect:**
```json
FFlagSampleFeature: true
FFlagAnotherFeature: false
```

### Claiming Credit

To claim credit for your contributions, add a comment at the **bottom of the JSON file (outside the brackets)**:

```json
{
  "FFlagFeature1": true,
  "FFlagFeature2": false
}
// #contributor-name
```

Replace `contributor-name` with your actual name or username.

---

## 🔐 Contributor Permissions

### Your Rights & Restrictions

- ✅ **Allowed:** Add and modify only your own FFlags files
- ✅ **Allowed:** Create new game folders and files
- ❌ **Restricted:** Edit other contributors' files
- ❌ **Restricted:** Delete other contributors' FFlags without permission

### File Ownership

Files are identified by the contributor name in the comment. Make sure to add your name to every file you create:

```json
{
  "FFlagMyFeature": true
}
// #my-name
```

---

## 📂 Repository Structure Example

```
Community-Fflags/
├── README.md
├── general.json          # General FFlags for all games
│
├── GameName1/
│   ├── place-id.ini      # Contains: 12345678
│   ├── fflags.json       # FFlags with #contributor-name
│   └── graphics.json     # FFlags with #contributor-name
│
└── GameName2/
    ├── place-id.ini      # Contains: 87654321
    └── fflags.json       # FFlags with #contributor-name
```

---

## 💡 Best Practices

- Use clear, descriptive FFlag names
- Keep related FFlags in the same file
- Always add your contributor name/comment
- Test your FFlags before submitting
- Provide context if the FFlag is for a specific feature

---

## ❓ Questions or Issues?

If you have questions about contributing or encounter any issues, please open an issue on this repository.

Happy contributing! 🎉
