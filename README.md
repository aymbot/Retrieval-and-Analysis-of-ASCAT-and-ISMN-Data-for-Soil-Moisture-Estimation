# Retrieval and Analysis of ASCAT and ISMN Data for Soil Moisture Estimation
This project aims to simulate a real world experiment for the course Data Stewardship *(UE 2023S)*

[![DOI](https://zenodo.org/badge/640369755.svg)](https://zenodo.org/badge/latestdoi/640369755)

## Table of Contents

- [Overview](#overview)
- [Data Sources](#data-sources)
- [Documentation and Data Management Plan (DMP)](#documentation-and-data-management-plan-dmp)
- [Code Execution](#code-execution)
- [License](#license)

## Overview
This is a project focused on retrieving and analyzing satellite-based ASCAT data and in-situ ISMN data for soil moisture estimation. 
By leveraging the H-SAF ASCAT SM CDR and ISMN data, the project explores the spatiotemporal dynamics of soil moisture and includes the calculation of Vegetation Optical Depth (VOD). 
Through the analysis of these datasets, the project aims to enhance our understanding of soil moisture dynamics and their implications for various applications such as agriculture, hydrology, and climate modeling.

## Data Sources

This project utilizes data from various sources. Detailed information about each data source, including metadata, data format, and any preprocessing steps, can be found in their respective folders within this repository.

### ASCAT Data

The ASCAT data used in this project is not included in this repository. To access the ASCAT data, you have two options:

1. **Fetch the data yourself**: Follow these steps to obtain the ASCAT data:
   - Visit the original data source [here](https://hsaf.meteoam.it/).
   - Download the data files in the required format (e.g., NetCDF).
   - Place the downloaded files in a newly created folder named `ascat_data` in the repository or local instance of yours.

2. **Reduced version on Zenodo**: Alternatively, you can use the reduced version of the ASCAT data that has been published on Zenodo. 
The Zenodo DOI for the reduced dataset is [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7932988.svg)](https://doi.org/10.5281/zenodo.7932988). To access the data, visit [here](https://zenodo.org/record/7932988#.ZGAEhqVBxD8) and download the dataset. If you choose this option, make sure to extract the data files and place them in the `ascat_data` folder.

#### Metadata and Format

The ASCAT data consists of the reduced ASCAT soil moisture data and relevant static layers such as terrain and soil porosity. The grid is also included, representing the grid information.
The metadata for the ASCAT data is as follows:

- Data Format: *NetCDF*
- Source Description: The ASCAT data is sourced from the EUMETSAT HSAF
- Data Origin: [see here](https://hsaf.meteoam.it/Products/Detail?prod=H120).
- Time Period Covered: The ASCAT data covers the time period 2011-2021

Please refer to the ASCAT source for more detailed metadata information about the ASCAT data.

### ISMN Data

The ISMN data used in this project is included in the `ismn_data` folder of this repository. The data files are already provided, and there is no need to fetch them from an external source.

#### Metadata and Format

The ISMN data provides in situ soil moisture measurements. The metadata for the ISMN data is as follows:

- Data Format: *csv* and *zip*
- Source Description: The ISMN data is sourced from the International Soil Moisture Network
- Data Origin: [see here](https://ismn.earth/en/dataviewer/).
- Time Period Covered: In the case of this experiment it will be temporarily matched with ASCAT data and result in the *matched_df* 

Please refer to the ISMN source for more detailed metadata information about the ISMN data.

## Documentation and Data Management Plan (DMP)

For further details on the data sources, metadata, and data management practices, please consult the Data Management Plan (DMP) associated with this project. The DMP provides comprehensive documentation, including information on data origin, characteristics, processing steps, and data access. 
The DMP is available on Zenodo, and the DOI is [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7933523.svg)](https://doi.org/10.5281/zenodo.7933523). You can access the DMP by visiting [here](https://zenodo.org/record/7933523#.ZGAPQaVBxD8).


## Code Execution

To run the code in this repository, you need **Python 3.8.10** installed on your system. Follow the steps below to set up the project and execute the source code:

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies by running the following command:
  ``` pip install -r requirements.txt ```
4. Open the Jupyter Notebook `experiment_notebook.ipynb` in your Jupyter environment.
5. Follow the instructions and documentation within the notebook to execute the code and reproduce the analysis.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).


