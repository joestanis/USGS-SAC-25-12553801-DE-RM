# Earthquake Data Visualization Tool
Developmental release v1.0

## Contact
Joseph Stanis, joestanis@gmail.com

## Project Overview
A sample tool built to satisfy the coding exercise for USGS Supervisory Computer Scientist vacancy USGS-SAC-25-12553801-DE-RM. This project is built using specific objectives while emphasizing code efficiency, readability, and adherence to best practices.

This project is tested to run inside Google Colab. It should also run in any environment with access to Project Jupyter, Python 3, and associated dependencies.

### Tool workflow
1. Read shake trace data from miniSEED files.
2. Instantiate a new SQLite database.
3. Extract the shake traces.
4. Transform and load the traces into the database.
5. Generate visual representations of the traces, collected samples, and collection site locations.

## Software Requirements
* Project Jupyter, free and available from https://jupyter.org/
* Python version 3, free and available from https://www.python.org/
* ObsPy library for Python, https://docs.obspy.org/, installable as a module via pip.
* Cartopy library for Python, https://scitools.org.uk/cartopy/docs/latest/, installable as a module via pip.

## Files Overview

### Scripts
* `JoeStanis_USGS_SeismicData.ipynb` - Jupyter notebook containing Python scripts which read and process the shake trace data.

### Data files
* `data/SEP01.mseed` - Earthquake shake data in miniSEED format.
* `data/SEP02.mseed` - Earthquake shake data in miniSEED format.
* `data/SEP03.mseed` - Earthquake shake data in miniSEED format.

### Other software release files
* `README.md` - This file, documents the project release version and overview information.
* `LICENSE.md` - Software release license and copyright.
* `DISCLAIMER.md` - USGS approved software release disclaimer.
* `CHANGELOG.md` - History of any project release revisions.
* `CODE_OF_CONDUCT.md` - Declaration to abide by the USGS Code of Scientific Conduct.
* `code.json` - USGS coding metadata describing the project.

### Output files
* `usgs_miniseed_data.sqlite.db` - SQLite database containing the ETL miniSEED data.
> [!TIP]
> If using Google Colab to run this notebook the generated database file should be accessible in the `Files` pane. 
> ![image](https://github.com/user-attachments/assets/eb0acc47-e147-4fed-92a6-d63292d57c81)

## Distribution
This project is released for public use, distribution is unlimited.
