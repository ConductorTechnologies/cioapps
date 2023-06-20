Congratulations! You're set to start submitting renders to Conductor from within Maya. Open Maya and load the Conductor plugin from the Plugin Manager. You should see a new menu called "Conductor" in the main menu bar. From there you can configure a submission.

### Shared installation

If you'd like to make the plugin accessible to others on your network, use one of the methods below:
1. Share the conductor.mod file with colleagues so they can add it to their Maya environment. You'll find it in your Maya prefs/modules folder.
2. Point the MAYA_MODULE_PATH environment variable to the Conductor install location as shown below.

```bash
# Add the Conductor module install location to the MAYA_MODULE_PATH.
export MAYA_MODULE_PATH={{installPath}}:$MAYA_MODULE_PATH
```