# ODBC Driver 18 Installation for Azure App Service on Linux

This repository provides a Dockerfile designed for deploying Python applications on Azure App Service using Linux, specifically configured to include the Microsoft ODBC Driver 18 for SQL Server. 

## Contents

- `Dockerfile`: Script to set up the Docker environment, including the installation of the Microsoft ODBC Driver 18.
- `odbc.ini`: Configuration file for setting up the ODBC driver.
- `requirements.txt`: File listing the Python packages required by the application (at least pyodbc)

The Dockerfile is prepared to set up a Python environment, install necessary system dependencies, and configure the ODBC driver for SQL Server connectivity. It includes:

- Installation of build tools, curl, and other utilities.
- Configuration of the Microsoft apt repository.
- Installation of the Microsoft ODBC Driver 18.
- Cleanup of apt caches to reduce the image size.
