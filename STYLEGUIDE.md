# project_m
## Style Guide
### General

Naming conventions files and folders:
folder names - upper snake case: Example_Folder_Name
gdscript and scene files - pascal case: ExampleScript.gd/ExampleScene.gd
other files (.json, .png) - lower snake case: example_image.png/example_resource.json

gdscript code:
functions - snake case: example_function()
signals - snake case, past tense: example_signal_happened
variables - camel case: exampleVariable
variables (loading a resource) - pascal case: ExampleScene
const and enum types - screaming snake case: EXAMPLE_CONST, EXAMPLE_ENUM.EXAMPLE_VALUE

**Static type wherever possible!** - exampleVar: ExampleClass
**Give return type wherever possible** - func example_function() -> void:

More general info [here](https://docs.godotengine.org/en/3.1/getting_started/scripting/gdscript/gdscript_styleguide.html#naming-conventions)

### Project Structure
project_m: the root folder (res://)
  Builds: any builds go here with the date/version number of the build
  Scripts
    Prefab_Scripts: scripts for all prefabs and reusable objects
    Scene_Scripts: scenes for the root node in each scene
    Global_Scripts: any auto-run scripts (managers)
  Scenes
    Menu_Scenes: menu scenes, simple 2D UI scenes like the main menu or options
    Game_Scenes: any scene involving the main game
  Prefabs: all reusable scenes or scenes that are not the root node, split by type depending on need
  Assets
    Images
    Music_And_Sounds
    etc...
