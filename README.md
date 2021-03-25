## Architecture

![Architecture](https://github.com/aniket-somwanshi/ai-based-quality-control/blob/master/Resources/architecture.jpeg)

###### The aim is to improve the Qualty Control in manufacturing units. The proposed architecture considers serveral end points in order to assess the quality of the current batch in production. The following feeder models are used for weighted probability estimation.

## Feeder Models
### Sensors Reliability
We rely on sensors for accuarate data. Although it's highly likely that the senor is malfunctioning, affecting the quality of the batch. Eg. Senors in underwater areas, often give out error reading. 
The <b> sensor_misreading_probability </b> is obtained from this model.

### Raw material Degradation
Raw materials are core components which may result in defects if are degraded, oxidized or expired. It is essential to asees the quality of raw materials that goes into the batch.
The <b> raw_material_degradation_proba </b> is obtained from this model.

### Human Error
As much as we want to replace human interaction, there are places where human inspection is mandatory. But, this defect inspection by human is likely to be false as well, depending on factors like time of the day, experience of worker, etc. This model gives us confidence score of the human's call.
The <b> human_error_proba </b> is obtained from this model.

### Defect Detection
This model analyses the composition, dimensions, structure of the product to ouput a probability of the batch being defective
 The <b> defect_proba </b> is obtained from this model.

## Final Estimation
Now we have the 4 feeder model's weighted probablities of a batch being defective. But the threshold after which we should flag the batch to be "defective" or "go to go" is still unknown.
We will decide the threshold using the <b> demand of the production </b> If the demand is low, we can afford to flag a "less likely defective" product to be "defective", just to be safe, as we have the time, since the demand is lower. Conversely, if the demand is very high, we cannot afford to do the same, as we don't have the time to "re-process" the batches. 


Thus, demand forecast helps decide the threshold after which we will flag the batch as "defective" or "go to go".



Conclusively, we have utilized all the above factors & touchpoints to improve quality control using Artificial intelligence.
