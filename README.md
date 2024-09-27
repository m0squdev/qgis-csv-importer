# QGIS CSV Importer

QGIS CSV Importer is a plugin for QGIS that allows users to import CSV files containing geographical data into their QGIS projects. This plugin simplifies the process of adding point and polygon data from CSV files to your maps.

## Features

- Import CSV files containing geographical data
- Create point and polygon layers from CSV data
- Automatically label imported features
- Simple and user-friendly interface

## Installation

1. Download the plugin files from this repository.
2. Place the files in your QGIS plugins directory.
3. Enable the plugin in QGIS through the Plugin Manager.

## Usage

1. Open your QGIS project.
2. Click on the CSV Importer icon in the QGIS toolbar or find it in the Plugins menu.
3. In the dialog that appears, select your CSV file using the file picker.
4. Click "OK" to import the data.

## CSV Format

Your CSV file should have the following columns:
- `label`: The label for each feature
- `coordinates`: Comma-separated coordinates for each feature
  - For points: `longitude,latitude`
  - For polygons: `lon1,lat1,lon2,lat2,lon3,lat3,...`

## Requirements

- QGIS 3.x
- Python 3.x
- pandas library

## Development

This plugin was generated with the help of the QGIS Plugin Builder. It consists of three main files:

1. `csv_importer.py`: The main plugin logic
2. `csv_importer_dialog.py`: The dialog class for the plugin
3. `csv_importer_dialog_base.ui`: The UI file for the plugin dialog

To modify the plugin, edit these files as needed. Remember to reload the plugin in QGIS after making changes.
