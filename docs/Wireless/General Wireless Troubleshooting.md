### Wireless Troubleshooting

**SNR (Signal-to-Noise Ratio)** is a ratio based value that evaluates your signal based on the noise being seen. SNR is comprised of 2 values and is measured as a positive value between **0db** and **120db** and the closer it is to 120db the better: signal value and noise value typically these are expressed in decibels (db).

**RSSI (Received signal strength indication) ** will look at the Signal (Also known as RSSI) first this value is measured in decibels from **0** (zero) to **-120** (minus 120) now when looking at this value the closer to 0 (zero) the stronger the signal is which means it's better, typically voice networks require a -65db or better signal level while a data network needs **-80**db or better. 

Normal range in a network would be **-45db to -87db** depending on power levels and design; since the signal is affected by the APs transmit power & antenna as well as the clients antenna.

 Signal strength (RSSI, “signal strength”, Signal/Noise Ratio.)  It’s generally best to focus on RSSI

1.  **RSSI < -90 dBm**: this signal is extremely weak, at the edge of what a receiver can receive.
2.  **RSSI -67dBm**: this is a fairly strong signal.
3.  **RSSI > -55dBm**: this is a very strong signal.
4.  **RSSI > -30dBm**: your sniffer is sitting right next to the transmitter.

**EXAMPLE:** Actual RSSI + Antenna Gain = Displayed RSSI  
                        ** -68db + 2db = -66db**

**NOISE** is any signal (interference) that is not WiFi traffic such as **cordless phones, microwaves, radar,** etc.This value is measured in decibels from **0 (zero) to -120** (minus 120) now when looking at this value the closer to -120 (minus 120) is better because that means there is little to no interference. Typical environments range between -90db and -98db.

**SNR calculation:**

     So to calculate your SNR value you add the **Signal Value to the Noise Value** and it generates a positive number that is expressed in decibels (db); 

**EXAMPLE:** lets say your Signal value is -55db and your Noise value is -95db.

                   **-55db + -95db = 40db** this means you have an SNR of 40, our general rule of thumb is that any SNR above **20** is good.

SNR calculations can be either simple or complex, and it depends on the devices in question and your available data. So, if your SNR measurements are already in decibel form, then you can subtract the noise quantity from the desired signal: SNR = S - N. This is because when you subtract logarithms, it is the equivalent of dividing normal numbers. Also, the difference in the numbers equals the SNR. For example, you measure a radio signal with a strength of -10 dB and a noise signal of -50 dB. -10 - (-50) = 40 dB.

**RSSI (Received Signal Strength Indicator)** is a more common name for the Signal value; meaning it is the strength that the device is hearing a specific device or signal. RSSI is most common used in bridge links where on client laptops they just call it **Signal**.

**EIRP (Effective Isotropic Radiated Power)** is the actual amount of signal leaving the antenna and is a value measured in db that is based on 3 things: **Transmit Power (db), Cable Loss (db), & Antenna Gain (dbi)**. To determine EIRP follow this equation: **Transmit Power - Cable Loss + Antenna Gain = EIRP**.

!**EXAMPLE:** We have a AP 124 access points running at full power with a 6dbi antenna on the 802.11a radio and a 2.5dbi antenna on the 802.11bg radio.

                            **802.11a EIRP = 17db (40mw) - 0db + 6dbi = 23db = 200mw** of actual output power

                            **802.11bg EIRP = 20db (100mw) - 0db + 2.5dbi = 22.5db = 150mw** (approx.) of actual output power, based on the example above in theory if you were to measure it right at the antenna you could get an RSSI of -23 or -22.5 respectively.

**Free Space Path Loss** is a measure of how much signal power you lose over a given distance typically you lose about 0.020 db per foot in an outdoor or wide open office; doors, walls, glass, and etc. affect this. This is why as you walk away from an AP your signal gets weaker.
