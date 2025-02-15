# Mass Spectrometry Peak Picking, Intensity Filtering, and Visualization

## Overview
This Python script processes mass spectrometry data by performing:
- **Peak Picking**: Extracts peaks around a specified m/z value.
- **Intensity Filtering**: Removes low-intensity signals below a threshold.
- **Data Visualization**: Plots mass spectrometry spectra within a chosen m/z range.

## Installation
Ensure you have the required dependencies installed:
```sh
pip install pandas matplotlib seaborn openpyxl
```

## Usage
1. **Prepare Your Data**: Place your mass spectrometry data in an Excel file (e.g., `Test.xlsx`). Ensure it has two columns:
   - `m/z` (Mass-to-charge ratio)
   - `Intensity`

2. **Run the Script**:
```sh
python ms_peak_filter_plot.py
```

3. **Customize Parameters** (Modify `main()` in `ms_peak_filter_plot.py`):
   - Set `target_mz` for peak picking (default: `411`)
   - Set `intensity_threshold` (default: `100000`)
   - Adjust `mz_min` and `mz_max` for visualization

## Output Files
- `peakpicked.xlsx`: Contains peak-picked data
- `Filtered_Data.xlsx`: Contains intensity-filtered data

## Example Plot
The script generates a plot of the mass spectrometry data within a selected m/z range.

## License
This project is open-source under the MIT License.


