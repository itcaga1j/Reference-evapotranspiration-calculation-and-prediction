# Reference-evapotranspiration-calculation-and-prediction
Calculation of the Penman-Monteith Evapotranspiration (FAO-56 Method)

Reference evapotranspiration ($ET_{o}$) is done by the FAO 56 Penman-Monteith method. This method is broadly accepted by the scientists around the world and it is used as the standard method to estimate the $ET_{o}$. The equation relies on conventional meteorological data concerning solar radiation (sunshine), air temperature, humidity, and wind speed.

Daily ETo was calculated by means of the FAO 56 PM equation:

$ET_{o} = \frac{0.408\Delta(R_n-G)+\gamma\frac{900}{T+273}u_2(e_s-e_a)}{\Delta + \gamma(1+0.34u_2)}$

where $ET_{o}$ is reference evapotranspiration (mm day $^{-1}$); $R_n$ is net radiation at the crop surface; $G$ is the soil heat-flux density ($MJ m^{-2} day^{-1}$); $T$ is the mean daily air temperature (°C) at a height of 2 m; $u_2$ is the wind speed at a height of 2 m ($m s^{-1}$); $e_s$ is the saturation vapor pressure (kPa); $e_a$ is the actual vapor pressure (kPa); ($e_s$ - $e_a$) is the saturation vapor pressure deficit (VPD) (kPa); $\Delta$ is the slope of the vapor pressure curve ($kPa ^\circ C^{-1}$); and $\gamma$ is the psychrometric constant ($kPa ^\circ C^{-1}$).

Relative Humidity: According to Allen et al, if there is no relative humidity data or the RH data is questionable quality, the RH ($e_a$) can be can be obtained by assuming when the air temperature is close to $T_{min}$, the air is nearly saturated with water vapor and the relative humidity is near 100\%,in other words, dewpoint temperature ($T_{dew}$) is near the daily minimum temperature ($T_{min}$). 

Wind Speed: According to Allen et al, if there is no wind speed data, it is acceptable to set value of wind speed to 2$ms^{-1}$ because that is the average wind speed for the 2000 main stations in the world. 

The purpose is to see how far are the reference evapotranspiration calculations on data without one perimeter from the calculations with the complete dataset.  Evapotranspiration will be evaluated in the following cases:

1. On the complete data set

2. No data on relative humidity

3. No wind speed data.

After comparing the calculations, reference evapotranspiration will be predicted on the complete dataset and evaluated using the evaluation metrics. 
