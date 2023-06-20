Congratulations! You're set to start submitting renders to Conductor from within 3d Studio Max.

* Open Max and choose **Rendering->Render With Conductor**.
### Shared installation

To make the 3ds Max Conductor plugin accessible to others on your network, ask them to create a file called ciomax_startup.ms in one of
their 3ds Max startup folders with the contents below.

```bash
-- Calls the Conductor 3DS Max plugin.
(
  include "{{installPath}}/Conductor.ms"
)
```