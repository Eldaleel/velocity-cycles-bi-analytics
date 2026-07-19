# SSAS project setup

This directory contains the reusable SQL Server Analysis Services multidimensional project used by the Velocity Cycles Power BI analysis.

## Requirements

- Visual Studio with the Microsoft Analysis Services Projects extension
- SQL Server Analysis Services in multidimensional mode
- A compatible `VelocityCyclesDW` SQL Server data warehouse

## Configure the data source

1. Open `Olapcube/Olapcube.dwproj` in Visual Studio.
2. Replace `YOUR_SQL_SERVER` in both `Olapcube.dwproj` and `Velocity Cycles DW.ds` with your SQL Server instance.
3. Confirm that the source database is named `VelocityCyclesDW` or update `Initial Catalog` accordingly.
4. Review impersonation settings for your environment, then deploy and process the cube.

The original `.bak` database backup is not included because it exceeds GitHub's standard 100 MB file limit. Visual Studio's user-specific `.dwproj.user` file is also excluded because it contains local machine settings.
