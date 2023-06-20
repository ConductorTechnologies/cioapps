Conductor core contains the Conductor client-side Python API along with a command-line tool to start the uploader and downloader daemons.

### Command-line usage

```bash
# Get help on the conductor command:
conductor --help
# Run the downloader daemon:
conductor downloader
# Run the uploader daemon:
conductor uploader
```

Python API

If you want to write tools against the Conductor Python client API, we suggest you install this package with Pip.



```bash
# Install the Conductor Python API:
pip install --upgrade {{packageName}}
```