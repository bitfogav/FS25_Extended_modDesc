# FS25_Extended_modDesc
FS25 extended modDesc template

# Extended modDesc

The XML file serves as both a configuration and metadata template for the mod, defining key details such as the author, version, localization, dependencies, maps, and more.

## Overview of `modDesc.xml`

The `modDesc.xml` file is structured with a root `<modDesc>` element and multiple child elements that define various aspects of the mod. Here’s a breakdown of the main sections:

### Author and Version
- **`<author>`**: Specifies the mod creator.
- **`<version>`**: Indicates the current version of the mod.

### Title and Description
- **`<title>`** and **`<description>`**: Provide the mod’s title and description in different languages (e.g., English `<en>` and German `<de>`), enabling localization.

### Icon and Multiplayer Support
- **`<iconFilename>`**: Points to the mod’s icon image file.
- **`<multiplayer>`**: Uses attributes like `supported` and `only` to specify the mod’s multiplayer capabilities.

### Store Items and Dependencies
- **`<storeItems>`**: Lists any additional store items related to the mod.
- **`<dependencies>`**: Enumerates other mods or files that this mod depends on.

### Localization (l10n)
- **`<l10n>`**: Contains language-specific text elements to support multiple languages, including localized `<text>` elements.

### Specializations, Maps, and Types
- **`<specializations>`**: Defines custom behaviors or features.
- **`<maps>`**: Contains one or more `<map>` elements. Each map includes attributes (such as filename, id, and configuration details) and localized titles and descriptions.
- **`<handToolTypes>`, `<placeableTypes>`, `<vehicleTypes>`**: Define various in-game objects with potential sub-specializations.

### Help Lines
- **`<helpLines>`**: Provides in-game help documentation with categories, pages, images, and text, guiding users through features or tutorials.

### Additional Configurations
- **`<extraSourceFiles>`**: Lists additional source files included in the mod.
- **`<parentFile>`**: Allows modifications to parent files by specifying attribute changes.
- **`<wildlife>`**: References configuration files related to wildlife modifications.

## Customization Instructions

1. **Replace Placeholder Text**  
   Replace all instances of `string` with your mod’s actual data (e.g., real author name, version number, titles, descriptions).

2. **Localization**  
   Update the `<en>` and `<de>` tags with your mod’s title and description translations. Additional languages can be added as needed.

3. **Define Dependencies and Specializations**  
   List any required mods or files in `<dependencies>`, and specify custom behaviors in `<specializations>` if your mod extends base functionality.

4. **Configure Maps and Game Elements**  
   Complete the `<maps>` section with appropriate filenames, IDs, and configuration details for each map. Similarly, configure sections for hand tools, placeable objects, and vehicles.

5. **Document Help Lines**  
   Use the `<helpLines>` section to provide players with in-game help, including images and descriptive text for guidance.

