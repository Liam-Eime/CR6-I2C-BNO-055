# CR6-I2C-BNO-055
Repository for my work with a Campbell Scientific CR6 data logger in CRBasic for I2C communication with a BNO-055.

### The Program
- Demonstrates reading/writing data from/to an I2C device; the BNO-055:
  - Reads the device chip ID.
  - Configures the units: Celcius for temperature, Degress for angles, rps for gyroscope, and mg for accelerometer.
  - Configures the operating mode to be 'NDOF', one of the fusion methods with all sensors available for reading.
  - Reads the raw accelerometer data; all three axes. This is done in the way of the Help documentation example.
  
- The current version of the program experiences the following potential issues:
  - The accelerometer readings seem to behave quite strange. This is likely due to how the raw data read in accel_tmp()
    'is being handled.
