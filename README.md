## Architecture

![Architecture](https://github.com/aniket-somwanshi/ai-based-quality-control/blob/master/Resources/architecture.jpeg)

###### The aim is to improve the Qualty Control in manufacturing units. The proposed architecture considers serveral end points in order to assess the quality of the current batch in production. 
##### The following feeder models are used for weighted probability estimation.

### Sensors reliability
We rely on sensors for accuarate data. Although it's highly likely that the senor is malfunctioning, affecting the quality of the batch. Eg. Senors in underwater areas, often give out error reading. 
The <b> sensor_misreading_probability </b> is obtained from this model.
