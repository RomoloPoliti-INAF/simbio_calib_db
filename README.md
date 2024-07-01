# SIMBIO-SYS Calibration Database


This is the repository of the calibration database for the SIMBIO-SYS Suite on board the ESA BepiColombo mission.

The database consists of three elements:
- The `version.yml` file, which contains the version number of the database
- The `calib_db.csv` file, which contains information about the calibration data and their scope of applicability (see the specific [section](#calibration-db-fields) for details)
- The `data` folder, which contains the calibration matrices


## Calibration schema

Will be implemented soon

## Calibration DB fields

- **Description** Description of the step (used for messaging and log)
- **Channel** SIMBIO-SYS channel to calibrate
- **Calibration_Step** name of the step will use the matrix
- **Size** size of the matrix (used for load the data)
- **Mask** value used to mask the pixel. If the value is 0 the mask will not applied.
- **Type** Is the data type of the values in the matrix.
- **Func** is the type of function will be used for the calibration. See specific section
- **Start** is the start date of validity of the matrix
- **End** is the end date of validity of the matrix. If the value is "*Now*" means that there is no end of validity.
- **File** is the path and the the name of the file containing the matrix.