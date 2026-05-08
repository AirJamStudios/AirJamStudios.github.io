# Guidelines
Little set of rules and preferences for working in a project :)

### Engine
For the development or our games we will be using [Godot](https://godotengine.org/download/linux/) version 4.6.2

### Folder structure
All projects should follow the following folders structure in the project root folder:

    assets/
        textures/
        models/
        audio/
        icons/
    resources/
        materials/
        shaders/
        ...
    scripts/
    scenes/
    
### Good practices:
1. When saving a scene, do not modify the transform of the root node
2. Prefer exported or cached node references over dynamic `get_node()` lookups
3. Keep scenes modular and reusable whenever possible
4. Keep one main responsibility per scene / script
5. Prefer composition over large monolithic scenes