Almost there! You just need to tell Clarisse where to find the Conductor plugin.

* Open Clarisse and go to Edit->Preferences->General, then enter the following in the Startup Script field.

```bash
$CIO_DIR/cioclarisse/startup.py
```

* Now restart Clarisse and find ConductorJob in the Create menu.

*In case you are wondering, CIO_DIR is a variable that has been added to your clarisse.env file.*
