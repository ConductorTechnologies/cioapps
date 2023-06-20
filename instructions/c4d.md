Almost there! You just need to tell Cinema4d where to find the Conductor plugin.

* Open Cinema4d and go to Edit->Preferences->Plugins.
* In the Search Paths panel click Add Folder, and browse to {{installPath}}.
* Restart Cinema4d and you should see a Conductor menu in the menu bar.

### Shared installation

If you'd like to make the plugin accessible to others on your network, without the need for them to install again, you can set Cinema4d's g_additionalModulePath environment variable. See below.


```bash
# # Add the Conductor plugin location to Cinema4d's g_additionalModulePath.
export g_additionalModulePath={{installPath}}:$g_additionalModulePath
```