---
tags:
  - it
  - python
---
The purpose of this setup is to configure the base environment needed to install and run Python packages

## Instructions

1. Install homebrew using the instructions in the [[Set Up Environment]] note

2. Install Python
```bash
brew install python@3.13
```

3. Setup a [virtual environment](https://docs.python.org/3/library/venv.html) in a directory of your choosing
```bash
python3.13 -m venv .venv
```

4. Install Python packages with:
```python
pip3 install <package name>
```