# test-doc

A test document repository with Sphinx documentation.

## Documentation

This repository contains basic Sphinx documentation for testing purposes.

### Building the Documentation

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Build the documentation:
   ```bash
   cd docs
   sphinx-build -b html source build
   ```
   
   Or using Make:
   ```bash
   cd docs
   make html
   ```

3. View the documentation by opening `docs/build/index.html` in your web browser.

### Documentation Structure

- `docs/source/index.rst` - Main documentation page
- `docs/source/installation.rst` - Installation guide
- `docs/source/usage.rst` - Usage guide
- `docs/source/conf.py` - Sphinx configuration

### Requirements

- Python 3.7 or higher
- Sphinx 9.0.0 or higher

