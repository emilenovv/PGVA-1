![image](https://user-images.githubusercontent.com/71296226/132027096-faaf05d9-d49e-4ffc-8519-34b66997d97f.png)

# **PGVA-1**
## **Decentralized Pressure and Vacuum Generator**

![Inkedpgva_award_new](https://user-images.githubusercontent.com/71296226/132029130-fff19bfa-6ae5-45ac-821d-e02f6f7329e7.jpg)

* Designed to supply Festo pipetting systems and liquid handling systems in the life sciences with compressed air and vacuum.
* The PGVA-1's usage can be extended to other areas as well to aspirate and dispense as a function of the pressure/vacuum levels generated by the PGVA.

## About
* This is an open software project which provides PGVA-1 customers and users with a wide array of driver templates in different coding languages to allow for quick and easy adaptability of the Festo pressure and vacuum generator to any system, project, or environment. Listed below are the current languages provided along with the methods that each driver provides to the user.

## Driver Languages
* [Python](examples/python)
* [Java](examples/java)
* [.NET/C#](examples/c#)

## Methods
* **Aspirate** -
  * Purpose:      Aspirates (creates a vacuum) at the given pressure for the given amount of time
  * Value Ranges: actuationTime = 0 to 1000 ms, pressure = -450 to 0 mBar
  * Arguments:    int actuationTime (ms), int pressure (mBar)
  * Returns:      void
* **Dispense** -
  * Purpose:      Dispenses (creates an output pressure) at the given pressure for the given amount of time
  * Value Ranges: actuationTime = 0 to 1000 ms, pressure = 0 to 450 mBar
  * Arguments:    int actuationTime (ms), int pressure (mBar)
  * Returns:      void
* **Calibration** -
  * Purpose:      Sets the maximum, minimum, and zero pressure set points
  * Value Ranges: NONE
  * Arguments:    void
  * Returns:      void
* **SetPumpPressure** -
  * Purpose:      Sets pressure and vaccum threshold values in mBar
  * Value Ranges: pressure = 0 to 550 mBar, vacuum = -550 to 0 mBar
  * Arguments:    int pressure (mBar), int vacuum (ms)
  * Returns:      void
* **ReadSensorData** -
  * Purpose:      Reads the actual vaccum, pressurem and output pressure values from the device in mBar
  * Value Ranges: NONE
  * Arguments:    void
  * Returns:      int[] data (data[0] = vacuum, data[1] = pressure, data[2] = output pressure)
