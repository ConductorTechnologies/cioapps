1. Open Unreal and log into Conductor.
2. Enable the Conductor plugin from the Unreal Plugins Window at **Edit>Plugins**.
3. Set up the executors under **Project Settings>Plugins-Movie Render Pipeline**:
    * Default Local Executor -> MoviePipelineConductorLocalEditorExecutor
    * Default Remote Executor -> MoviePipelineConductorRemoteExecutor
    * Default Executor Job -> ConductorMoviePipelineExecutorJob
4. Add a new **Data Asset>Conductor Settings** asset to your Content Browser to configure your upload settings.
5. Optionally, set up a Perforce server.
    * Connect to the P4 Server, set up a P4 Workspace, and configure the Source Control plugin under **Tools>Revision Control**.
    * Add the following variables to your Conductor Data Asset's Environment Settings: P4PORT, P4USER, P4PASSWD.
6. Select your Conductor Settings via the **Movie Render Queue** and click Render (Remote) to submit.