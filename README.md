Hi Everyone

I’m Fateme, an environmental specialist passionate about air quality modeling.  
While working on atmospheric dispersion modeling with AERMET, I faced challenges processing raw meteorological data to meet input requirements.  
To solve this, I developed scripts to clean, organize, and prepare the data — filling gaps, aligning timestamps, and converting intervals to hourly records.  
I’m sharing this in case it helps others working on similar projects...

# aermet-meteorological-data-processing

This repository contains a collection of Python scripts designed to preprocess meteorological data for use in AERMET, a meteorological preprocessor for the AERMOD air dispersion modeling system. The scripts handle various data preparation tasks, including cleaning, filling missing values, and aligning timestamps to ensure the data meets the requirements for air quality modeling.

## Features

- **File Loading and Integration:**
  - Load meteorological data from Excel files.
  - Handle multiple years of data seamlessly.

- **Date and Time Management:**
  - Generate complete date ranges based on the Shamsi (Solar Hijri) calendar.
  - Convert 10-minute interval data to hourly intervals.
  - Ensure all expected date-time entries are present, filling any missing timestamps.

- **Data Cleaning and Imputation:**
  - Fill missing temperature values with 0.
  - Replace missing wind direction values with the most frequent direction.
  - Fill other missing meteorological parameters with the column mean.

- **Google Drive Integration:**
  - Load data directly from Google Drive for easy access and collaboration.

- **Output and Saving:**
  - Save the processed and cleaned dataset as a new Excel file.

## Workflow

1. **Load Data:** Import your meteorological dataset.
2. **Generate Date Range:** Create a complete date-time index.
3. **Merge Data:** Combine the generated date range with the existing dataset.
4. **Fill Missing Values:** Automatically fill gaps in the data.
5. **Save Processed Data:** Export the cleaned and complete dataset.

## Usage

1. Upload your meteorological data file (in Excel format) to your working environment.
2. Update the file path in the script (`path_to_your_file.xlsx`).
3. Run the script in a Python environment (e.g., Google Colab, Jupyter Notebook).
4. Download the processed file for use in AERMET.

## Example Output

After running the script, you’ll get a complete, gap-free dataset with hourly intervals, ready for direct use in AERMET for air quality modeling.

## Why This Is Useful

Accurate meteorological data is crucial for air dispersion modeling. Missing values, inconsistent timestamps, or incomplete date ranges can lead to inaccurate results. These scripts automate the cleaning and preparation process, saving time and ensuring high-quality inputs.

---

If you want me to tweak anything or add more details, just let me know! ✨


