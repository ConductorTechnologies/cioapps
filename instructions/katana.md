Congratulations! You're set to start submitting renders to Conductor from within Katana. Open Katana and select **Util->Conductor** to open the dialog. You can also right-click over a **Render** node and choose **Conductor** from the **Render Farm** section.


### Shared installation

To make the plugin accessible to others on your network:

* Open the Log view and look for the line "Wrote ConductorRender init file: `<path-to-katana-resources>/SuperTools/ConductorRender/__init__.py`
* Copy that file to the same location on other machines.
* Alternatively, make sure everyone has the KATANA_RESOURCES variable pointing to that location. 
