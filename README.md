# The tracebase data set

The tracebase data set is a collection of power consumption traces which can be used in energy analytics research. Traces have been collected from individual electrical appliances, at an average reporting rate of one sample per second.

Traces in the three directories *complete*, *incomplete*, and *synthetic* were collected in the city of Darmstadt, Germany, in 2012.
A second (much smaller) set of files has been collected in Sydney, Australia, in the year 2013 and is stored in the *australia* directory.

# Trace format

The collected readings are stored in comma-separated value files; one file is created for each metered wall outlet. Files are grouped into directories according to the type of the appliance that has been monitored. Each entry in the file contains the date and time of its collection and the power consumption readings averaged over time durations of one and eight seconds, respectively. The timestamp field follows the "day/month/year hour:minute:second" format, in which the time is specified using a 24-hour notation. An excerpt of a trace looks as follows:

```
14/01/2012 10:48:47; 151; 156
14/01/2012 10:48:48; 147; 151
14/01/2012 10:48:49; 147; 151
14/01/2012 10:48:50; 145; 149
14/01/2012 10:48:51; 145; 147
14/01/2012 10:48:52; 145; 147
14/01/2012 10:48:53; 143; 147
14/01/2012 10:48:54; 143; 145
14/01/2012 10:48:55; 143; 143
```

# Trace files

The tracebase data set contains power traces of a variety of electric appliances. Traces are clustered into directories according to their collection process.


### Full-day traces

The "complete" directory contains traces which were recorded over a period of 24 hours. Each trace starts at midnight and ends at midnight the next day. The smart plug was not disconnected during this period even if the device had been switched off.

### Incomplete traces

This archive contains traces where measurement points are missing from the recorded data. This is mostly due to problems with the collection setup and/or the wireless transmission of the meter readings. No interpolation has been applied to traces in the "incomplete" folder. 

### Synthetic traces

The "synthetic" archive contains trace fragments of real appliances, which have been padded with zero consumption readings. The traces have been collected as follows: An appliance, e.g., a vacuum cleaner, has been connected
to the metering device at some point during the day (the usage time reflects the time during which the user wanted to use the vacuum cleaner) and was operated as usual. After it had been used, it was disconnected from the metering device. The resulting CSV file was thus composed of an incomplete daily trace, lacking both the periods before and after the usage of the appliance. These missing timeframes were artificially padded with zero consumption readings in order to attain a complete daily trace.

### Australia

Traces collected in Sydney, Australia, were not separated into the three aforementioned categories due to the small size of the data set.

# Using the data set

This data set is made available under the Open Database License: <http://opendatacommons.org/licenses/odbl/1.0/>. Any rights in individual contents of the data set are licensed under the Database Contents License: <http://opendatacommons.org/licenses/dbcl/1.0/>

Downloading the tracebase data set implies that you agree to the following conditions:

* When you use the tracebase data set in your scientific publications, you agree to add a citation of the following literature reference: **Andreas Reinhardt, Paul Baumann, Daniel Burgstahler, Matthias Hollick, Hristo Chonov, Marc Werner, Ralf Steinmetz: *On the Accuracy of Appliance Identification Based on Distributed Load Metering Data*. Proceedings of the 2nd IFIP Conference on Sustainable Internet and ICT for Sustainability (SustainIT), 2012.**
* When you use the tracebase data set in other activities, you agree to provide an attribution as part of your product: **Contains information from the tracebase data set, which is made available at http://www.tracebase.org under the Open Database License (ODbL).**

# Publications 

The tracebase data set has initially been presented in the following publication:

Andreas Reinhardt, Paul Baumann, Daniel Burgstahler, Matthias Hollick, Hristo Chonov, Marc Werner, Ralf Steinmetz: *On the Accuracy of Appliance Identification Based on Distributed Load Metering Data*. Proceedings of the 2nd IFIP Conference on Sustainable Internet and ICT for Sustainability (SustainIT), 2012. [[Paper](https://www.areinhardt.de/publications/2012/Reinhardt_SustainIt_2012.pdf)]

More publications about our smart metering activities in general and the use of appliance-level data are listed as follows:

Christoph Klemenjak, Andreas Reinhardt, Lucas Pereira, Mario Berges, Stephen Makonin, Wilfried Elmenreich: *Electricity Consumption Data Sets: Pitfalls and Opportunities*. Proceedings of the 6th ACM International Conference on Systems for Energy-Efficient Buildings, Cities, and Transportation (BuildSys), 2019. [[Paper](https://www.areinhardt.de/publications/2019/Klemenjak_BuildSys_2019.pdf)]

Alaa Alhamoud, Felix Ruettiger, Andreas Reinhardt, Frank Englert, Daniel Burgstahler, Doreen Böhnstedt, Christian Gottron, Ralf Steinmetz: *SMARTENERGY.KOM: An Intelligent System for Energy Saving in Smart Home*. Proceedings of the 3rd IEEE International Workshop on Global Trends in Smart Cities (goSMART), 2014. [[Paper](https://www.areinhardt.de/publications/2014/Alhamoud_goSMART_2014.pdf)]

Frank Englert, Till Schmitt, Sebastian Kößler, Andreas Reinhardt, Ralf Steinmetz: *How to Auto-Configure Your Smart Home? High Resolution Power Measurements to the Rescue*. Proceedings of the 4th International Conference on Future Energy Systems (ACM e-Energy), 2013. [[Paper](https://www.areinhardt.de/publications/2013/Englert_eEnergy_2013.pdf)]

Andreas Reinhardt, Dominic Burkhardt, Manzil Zaheer, Ralf Steinmetz: *Electric Appliance Classification Based on Distributed High Resolution Current Sensing*. Proceedings of the 7th IEEE International Workshop on Practical Issues in Building Sensor Network Applications (SenseApp), 2012. [[Paper](https://www.areinhardt.de/publications/2012/Reinhardt_SenseApp_2012.pdf)]

Andreas Reinhardt, Dominic Burkhardt, Parag Mogre, Manzil Zaheer, Ralf Steinmetz: *SmartMeter.KOM: A Low-cost Wireless Sensor for Distributed Power Metering*. Proceedings of the 6th IEEE International Workshop on Practical Issues in Building Sensor Network Applications (SenseApp), 2011. [[Paper](https://www.areinhardt.de/publications/2011/Reinhardt_SenseApp_2011.pdf)]

# Contact

tracebase is a collaborative project of the [Multimedia Communications Lab (KOM)](https://www.kom.tu-darmstadt.de) and the [Secure Mobile Communications Lab (SEEMOO)](https://www.seemoo.tu-darmstadt.de/home-vision/) at Technische Universität Darmstadt, Germany, as well as the [Department of Informatics (IfI)](https://www.in.tu-clausthal.de) at Technische Universität Clausthal, Germany.

Please contact our team at info *at* tracebase *dot* org if you have further questions.
