# plugins-api  

DRC plugin repository.  

# Contribute a Plugin  

Create a pull request to this repository, containing:  

- Your plugin information in `registry.json`, under `list`  
- A directory with a name corresponding to your plugin `id` as in `registry.json`.
- Add a file in your directory containing a file called `plugin.json`.  
- This is hosted on GitHub Pages, so you can host your assets on https://deeeep-reef-client.github.io/plugins-api/[PLUGIN ID]  

Plugins contributed must be licensed under the [Unlicense](https://unlicense.org).  

## Plugin Info Template  

```json
{
    "name": "Your Plugin Name",
    "id": "a-unique-id",
    "type": "plugin **OR** theme",
    "description": "Your plugin description",
    "author": "Your name :)"
}
```

## Script Plugin  

### Explanation:  

Type:  

- `startup`: Executes code on app startup in index.js  
- `preload`: Executes code on preload.js start  
- `domloaded`: Executes code on DOM content loaded after all DRC scripts have run  
- `game`: Executes in main world after game has loaded. Will have access to game API but will NOT have access to Node  

```json
{
    "name": "Your Plugin Name",
    "id": "a-unique-id",
    "description": "Description of your plugin",
    "author": "Your name",
    "type": "startup **OR** preload **OR** game **OR** domloaded",
    "src": "JavaScript source that will be executed"
}
```

## Themes  

If you realised this is the exact format you get when using the built in export feature, so you can just paste it in and change its name.  
```json
{
    "name": "Name of your theme",
    "src": "CSS source"
}
```