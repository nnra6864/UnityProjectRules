# General
- Don't use spaces when naming things
- Don't use any special characters when naming stuff(this includes other languages)
- Don't add any unnecessary files to the project directory, keep it clean and keep in mind that github offers limited space(2GB)
- When exporting models, pngs etc. there is no need to export them to the `Krita`/`Blender` directory, export them directly to `Assets/AppropriateDir` to avoid duplication
- Every asset should have the proper suffix added to their name, an example would be `BackgroundImage.png` instead of `Background.png`

# Project Structure
```
ProjectName
├── Git
├── Builds
│   ├── Android
│   ├── Linux
│   └── Windows
└── Project
    ├── Blender
    ├── FLStudio
    ├── Krita
    └── Unity
        └── ProjectName
            ├── Assets
            │   ├── Scripts *Divide into namespaces*
            │   ├── Materials
            │   ├── Sounds
            │   │   ├── SFX
            │   │   └── Music
            │   ├── Sprites
            │   ├── Prefabs
            │   ├── Scenes
            │   ├── Shaders
            │   ├── VFX
            │   ├── Animations
            │   ├── Miscellaneous
            │   ├── Models
            │   └── Textures
            ├── Packages
            └── ProjectSettings
```
# Software
**Game Engine** - Unity <br/>
**IDE** - Optional <br/>
**Image Editing** - Krita <br/>
**Modelling** - Blender <br/>
**SFX**/**Music** - Optional <br/>

# C`#`
## General
- Always use namespaces, you can add the current `class` to the proper `namespace` by placing cursor over the `class name`, clicking `ctrl`+`.` and adding it to the namespace
- Add the **type suffix** to **properties**, **fields** and **variables**, example of that would be `playerTransform` instead of `player`
## Naming Conventions
- Namespace `CamelCase`
- Class `CamelCase`
- Private Field/Property `_camelCase`
- Public Field/Property `CamelCase`
- Method `CamelCase`
- IEnumerator `CamelCase`+`Routine`
- Coroutine `_camelCase`+`Routine`
- Parameters/Variables `camelCase`
## Declaration Order
- This is optional but if you don't have your own rules, follow this:
```
Constants
Private Fields
Public Fields

Serialize Fields

Private Properties
Public Properties

Unity Functions

Private Functions
Public Functions
```
