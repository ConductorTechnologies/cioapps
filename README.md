# cioapps

A repository containing resources to configure Plugins hosted in the Companion app.

### Index file

The file `index.json` contains a list of metadata objects representing the apps that are available to be installed from the Companion app. Each entry describes the app's name, description, registry source and so on.

### Descriptions folder

The folder `descriptions` contains text files that are used to populate the app descriptions on the cards in the Companion app Plugins page. The files are named after the app's name, and the contents of the file are used as the description. They have the `.md` extension, but they are not treated as markdown files in the app.

### Instructions folder

The folder `instructions` contains markdown files that are used to populate the app instructions on the popup cards that appear after a plugin has been installed. The files are named after the app's name, and the contents of the file are used as the instructions. 

They are treated as Markdown files in the app and converted to React components, however it is not recommended to use all Markdown features, as only some are recognized for styling. In particular, it's best not to use any other headers than `###`. See the files in the folder for examples.

The instructions files can contain placeholders that are replaced with values from the app at installation time.


| Placeholder | Description | Example |
| ----------- | ----------- | ------- |
| `{{packageLocation}}` | The Conductor folder as configured on the settings page | /Users/jmann/Conductor |
| `{{pluginName}}` | The name of the plugin | maya |
| `{{packageName}}` | The name of the package | ciomaya |
| `{{installPath}}` | The full path where the plugin is installed | /Users/jmann/Conductor/maya/ciomaya |

