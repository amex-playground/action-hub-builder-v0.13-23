# hub-builder

A simple interface for recursively building & validating Hub executors. Built on top of `jina hub` interface. This will serve as the core of our Github action/bot, CICD workflow.

## Install

```bash
pip install -r requirements.txt
python app.py --help
```

## Usage

### Recursively Build All Executors in `/abc`

```bash
python app.py /abc
``` 

### Recursively Check All Executors in `/abc` Without Building

```bash
python app.py /abc --dry-run
```

Note that `dry-run` only checks the name conventions, required files. No actual testing and building. 

### View the Build Log of a Run

Simply open the `build-TIMESTAMP.json`, there you have a complete overview of this build round and details of each executors.
