## Architecture

![Architecture](https://github.com/aniket-somwanshi/ai-based-quality-control/blob/master/Resources/architecture.jpeg)

###### The aim is to improve the Qualty Control in manufacturing units. The proposed architecture considers serveral end points in order to assess the quality of the current batch in production. 
###### The following feeder models are used for weighted probability estimation.

### Sensors Reliability
We rely on sensors for accuarate data. Although it's highly likely that the senor is malfunctioning, affecting the quality of the batch. Eg. Senors in underwater areas, often give out error reading. 
The <b> sensor_misreading_probability </b> is obtained from this model.

### Raw material Degradation
Raw materials are core components which may result in defects if are degraded, oxidized or expired. It is essential to asees the quality of raw materials that goes into the batch.
The <b> raw_material_degradation_proba </b> is obtained from this model.

### Human Error
As much as we want to replace human interaction, there are places where human inspection is mandatory. But, this defect inspection by human is likely to be false as well, depending on factors like time of the day, experience of worker, etc. This model gives us confidence score of the human's call.
The <b> human_error_proba </b> is obtained from this model.

### Raw material Degradation
Raw materials are core components which may result in defects if are degraded, oxidized or expired. It is essential to asees the quality of raw materials that goes into the batch.
The <b> raw_material_degradation_proba </b> is obtained from this model.
