# Wakefield Raceway GPS Project

## Overview
This project reconstructs a car’s path around Wakefield Park Raceway using GPS data.  
The script reads a CSV file exported from the GPS unit, groups points by lap, and creates a polyline shapefile with one feature per lap.

## Requirements Met
- Used Python’s `csv` module to parse the dataset
- Handled comment lines and session markers
- Grouped points by lap number
- Created a shapefile in WGS84 with a Lap field
- Produced one polyline per lap

## Reflection
See [reflection.md](reflection.md) for a detailed write‑up of what I learned and the challenges I overcame.

## Over and Above
- Debugged file path and format issues (CSV vs Excel)
- Adjusted script to match exact column names
- Added optional thinning parameter to reduce point density

## How to Run
1. Save the Excel file as CSV (Comma delimited).
2. Update the `input_csv` and `output_workspace` paths in the script.
3. Run the script in ArcGIS Pro’s Python environment.
4. The output shapefile will contain one polyline per lap.
