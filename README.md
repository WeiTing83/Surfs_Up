# Surfs_Up

### Overview of the analysis:
    W. Avy evaluates opening surf shop in Oahu. She wanted to analyze temperature data for the months of June and December, in order to determine if the surf shop business is sustainable for whole year. Thus, she used Python, Panda and SQLAlchemy to analyze the weather data in Hawaii. 
>
### Definition of Data: 
+ The station detected the data about precipitation and temperature. Because the station can measure precipitation, we suppose the temperature should be air temperature, not ocean temperature. 
+ We don’t consider ambient condition, such as wind, sun, humidity and so on.
+ Our temperature is air temperature so ocean temperature must be lower than our measured data.
+ The air temperature is between 85 and 70F suitable for surf.
>
### Results: 
#### <Table1. Temperature in June >
![JUNE]()
#### <Table2. Temperature in December >
![DEC]()

|                    | JUNE                           |DECEMBER                         |
|-------------------------------------|
|Year            | 2010-2017                    |2010-2016                 |
|Total Data   |1700                              |1517                          |
|temp. mean |  74.9F                                |71.0F;close to 70             |
|surfing    | comfortable      | probably feel cold           |
>
### Summary: 
The result shows, in December, the ocean temperature is a little bit cold and not suitable for surfing. However, in addition to ocean temperature, we should consider more factors which would potentially impact the surfing shop business, such as ambient condition and traveling seasons.
First, we need to consider ambient condition. For example, if the weather is sunny during winter, ocean temperature may not be too cold to significantly impact surfing shop business. Thus, to develop a sustainable business, we can do query for precipitation and check the weather condition based on Hawaii.sqlite. Then, we can further sort out weather conditions more locally based on meteorological data from local stations.  However, this precipitation database isn’t very clear because we also need to consider when the precipitation happened during daytime or nigh time. Second, this data recorded in Hawaii.sqlite is ambient temperature. For surfing activity, we should check ocean temperature which is an appropriate factor to evaluate when is good for surfing activity. Finally, during traveling season, except for the existing surfing shop business, we can develop a small business to provide more options to attract more customers, such ice cream shop and coffee shop.
--------------------------------------------------------------------------------------



Hawaii.sqlite has two tables,measurement and station.
Measurement has ID, station', 'date', 'prcp', 'tobs,

