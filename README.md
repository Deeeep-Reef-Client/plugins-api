# plugins-api  

DRC plugin repository.  

# Contribute a Plugin  

## NOTE: Plugins are NOT IMPLEMENTED yet  

Create a pull request to this repository, containing:  

- Your plugin information in `registry.json`, under `list`  
- A directory with a name corresponding to your plugin `id` as in `registry.json`, containing a `manifest.json` and all your assets  

## Plugin Info Template  

```json
{
    "name": "Your Plugin Name",
    "id": "a-unique-id",
    "type": "plugin",
    "description": "Your plugin description",
    "author": "Your name :)"
}
```

## Manifest.json  

```json
{
    // Insert Plugin Info Template
    "entry": "pluginentrypoint.js",
    "assets": [
        "myasset.js",
        "img/myimage.png"
    ]
}
```
