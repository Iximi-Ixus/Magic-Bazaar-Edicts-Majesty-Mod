# Magic Bazaar Edicts

A Majesty: The Fantasy Kingdom Sim modification that adds a new building to globally control Bazaar item availability.

## Overview

Magic Bazaar Edicts introduces the **"Bazaar is closed"** building, which provides players with complete control over when heroes can access Bazaar items. This mod allows for strategic gameplay by letting you disable all Bazaar purchases during critical moments or when you want to encourage alternative hero development paths.

## Features

- **Global Bazaar Control**: Build the "Bazaar is closed" building to disable all Bazaar items simultaneously
- **Strategic Flexibility**: Destroy the building to instantly restore access to all Bazaar items
- **Unique Building**: Only one "Bazaar is closed" building can exist at a time
- **Player Feedback**: Clear chat messages notify you when the Bazaar status changes
- **Non-Intrusive**: Doesn't affect existing save games or other mods

## How It Works

### Building the Edict
1. Construct the "Bazaar is closed" building (costs 10 gold)
2. Upon completion, all Bazaar items become unavailable to all heroes
3. The building type becomes disabled to prevent multiple instances
4. A chat message confirms: "Bazaar is closed"

### Revoking the Edict
1. Destroy the "Bazaar is closed" building
2. All Bazaar items become available again
3. The building can be reconstructed if needed
4. A chat message confirms: "Bazaar is open"

## Installation

1. **Copy to Game Directory**: Copy the entire `Magic Bazaar Edicts` folder to your Majesty's `MODS` directory
   - Usually located at: `C:\Program Files (x86)\Steam\steamapps\common\Majesty\MODS\`
   - Or: `C:\Program Files\Majesty Gold HD\MODS\`

2. **Launch Game**: Start Majesty with the expansion pack
3. **Enable Mod**: The mod will appear in your mod list as "Bazaar Edicts"
4. **Start New Game**: The mod requires a new game to take effect

## Files Structure

```
Magic Bazaar Edicts/
├── BazaarEdicts.mmxml          # Main mod configuration
├── BazaarEdicts.bcd            # Compiled GPL scripts
├── BazaarEdicts.mswproj        # Project file
├── BazaarEdict.png             # Mod icon
├── README.md                   # This file
├── LICENSE                     # MIT License
├── Data/
│   ├── EdictBuildngs.xml       # Building definitions
│   └── EdictText.xml           # Text strings
├── GPL/
│   ├── BirthDeathFunctions.gpl # Building lifecycle scripts
│   ├── DefinitionsAndHelperFunctions.gpl # Core functions
│   ├── ModifiedBazaar_Item_Check.gpl # Item availability logic
│   └── EdictBuildings.dat      # Building data
└── TempProject.gplproj         # GPL project file
```

## Technical Details

### GPL Implementation
- **Attributes**: Uses global attributes on the GPL AI Root to track Bazaar item states
- **Helper Functions**: Modular functions for enabling/disabling all items at once
- **Event Handlers**: Birth and death scripts handle building construction/destruction
- **Player Feedback**: Local chat messages provide immediate status updates

### Building Properties
- **Cost**: 10 gold
- **Health**: 10 HP (vulnerable to attack)
- **Appearance**: Uses the "BBs7" building sprite
- **Construction**: Available through standard building menu

## Compatibility

- **Game Version**: Requires Majesty: The Fantasy Kingdom Sim (Expansion recommended)
- **Other Mods**: Should be compatible with most mods that don't alter Bazaar mechanics
- **Save Games**: Not compatible with existing save games - requires new game

## Development

### Requirements
- Majesty GPL Compiler (`Gplbcc.exe`)
- Text editor for GPL scripting
- XML editor for data files

### Building from Source
1. Modify GPL files in the `GPL/` directory
2. Run `MakeGPL.bat` to compile scripts
3. Test in game environment
4. Package all files for distribution

## Credits & Attribution

### Original Game
- **Majesty: The Fantasy Kingdom Sim** - Owned by **Paradox Interactive**
- **Original Development**: Cyberlore Studios (1996)
- **Gold HD Edition**: Developed by 1C Company with modern platform updates
- **Steam Distribution**: Provided by Paradox Interactive

### Mod Creation
Created for the Majesty modding community.

**Special Thanks:**
- Dracoceros for initial modding guidance
- Enerril for GPL scripting and building creation assistance
- The entire Majesty modding community for sharing knowledge and examples

### Steam Workshop
- **Workshop Item ID**: 3554788619
- **Distribution**: Official Steam Workshop platform
- **Support**: Use the Workshop discussion section for mod-specific questions

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Steam Workshop Distribution

This mod is available on the official Steam Workshop:

- **Workshop Item ID**: 3554788619
- **Download**: Search for "Magic Bazaar Edicts" on Steam Workshop
- **Installation**: Subscribe through Steam (automatic installation)
- **Updates**: Steam handles automatic updates when available
- **Support**: Use the Workshop discussion section for questions and feedback

### Legal & Compliance Information

This is an **unofficial fan modification** that:
- ✅ Complies with Steam Workshop Terms of Service
- ✅ Follows the game's End User License Agreement (EULA)
- ✅ Does not modify or redistribute original game files
- ✅ Uses only the provided GPL scripting tools
- ❌ Is not officially supported by Paradox Interactive or 1C Company
- ❌ May not be compatible with future game updates

**Important**: You must own a legal copy of Majesty Gold HD through Steam to use this mod.

## Support

### For Mod-Specific Issues:
1. Check the Steam Workshop discussion section
2. Ensure you're using the latest version from Workshop
3. Verify game and mod compatibility

### For Game-Related Issues:
1. Contact official Steam support
2. Check game forums for known issues
3. Ensure your game is up to date

### Troubleshooting:
1. Ensure the mod files are in the correct directory
2. Verify you're running a new game (not loading an old save)
3. Check that the expansion pack is active
4. Review game logs for any GPL compilation errors
5. Try unsubscribing and re-subscribing to the Workshop item

---

**Note**: This mod enhances gameplay by adding strategic depth to Bazaar management. Use it to create challenging scenarios where heroes must rely on their natural abilities rather than purchased enhancements!

**Remember**: By using this mod, you agree to respect the intellectual property of Paradox Interactive and comply with all applicable terms of service.
