# ETL-Three-Datasets-Using-NumPy-and-Pandas
This is a nice example of performing ETL to combine three datasets to prepare a dataset for ML pipeline using NumPy and Pandas. This project was with Alberta Machine Intelligence Institute.

Ask me for the datasets if you want to work on it.

In this notebook, you will perform a number of steps that come up in the process of preparing the data to be used by a machine learning algorithm.

The main data was gathered from an experimental sensor device oserving an electro-chemical plant. The sensor device detects "interesting" events. These events were labeled by an expert into four different classes `"P"`, `"N"` and `"L"`  as well as `"-"`, which denotes a false detection (not an "interesting" event). The data shows readings for 9 different sensors along with a 'detection mode'&mdash;which affects the class of detected phenomenon&mdash; along with the date annd time when events happened. 

However, the expert also indicated that multiple factors affect the sensor readings as well. The fecators can be put into two broad categories: weather conditions where the device was used and the calibration of the device itself. For this reason, we gathered two more datasets to be used alongside the main data: 

One shows daily averages of three different weather indicators: temperature, humidity and wind level in the area the device was opertaing, as the expert indicated these may be the most relevant factors.

The other dataset is acquired from the logs of the maintenance done on the device: Every week at midnight on Friday, the device was turned off and inspected by a technican in the foloowign day. If the device was found to be near-faulty (indicated from certain measurements taken from device), the device was repaired and recalibrated. Again, the expert indicated three different measurements from the device that might be affecting the sensor readings. The device was turned back on again on midnight on Saturday.
