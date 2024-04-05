Conductor Core contains the the following:

* Conductor command line tools to start the uploader and downloader background processes and more.
* The `ciocore` client-side Python API, which allows you to integrate Cunductor into your own pipeline.

### Important notice. 

If you have installed Conductor Core version 8.0.0 or higher through this interface, the command line tools will not be available since it is now designed to be installed as a regular Python package.

You have three options to fix this: We strongly recommend the first option.

1. Go to [www.conductortech.com](https://www.conductortech.com/companion) and download the latest version of the Conductor Companion. The comnmandline tools are then installed automatically as a Python package during the Companion installation and become available from any terminal.

2. Add the path to the Conductor Core package to your PYTHONPATH. To do this, you can add the following to your `~/.bashrc` or `~/.bash_profile` on Mac or Linux:

```bash
export PYTHONPATH=$PYTHONPATH:{{packageLocation}}/{{pluginName}}
```

Then, open a new shell or run `source ~/.bashrc` or `source ~/.bash_profile` to apply the changes.

If you are using Windows, you can add the following to your `PYTHONPATH` environment variable in the Environment Variables settings:

```bash
{{packageLocation}}\{{pluginName}}

```

Now you should have access to the command line tools for ciocore version `8.0.0` or higher from any terminal. Type: `conductor --help` to test.

3. Choose to install one of the 7.x versions of Conductor Core from the menu. To aviod conflicts, we recommend you uninstall the current version of Conductor Core before installing the 7.x version. To do this, delete: `{{packageLocation}}/{{pluginName}}`

### Command-line usage

```bash
# Get help on the conductor command:
conductor --help
```

### Python API

If you want to write tools against the Conductor Python client API, we suggest you install this package with Pip.


```bash
# Install the Conductor Python API:
pip install --upgrade {{packageName}}
```
