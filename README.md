# Parkinson-Disease-Datasets

This repository contains datasets collected using sensor devices or microphones that can be used for the evaluation of Parkinson's disease (PD) motor symptoms or voice. This repository contains two main table describing characteristics of the datasets, the first containing information about the collection of the data and the other containing information like the size, language, and year of creation of the datasets. After these tables, the datasets are explored in more detail.

Unified Parkinson's Disease Rating Scale (UPDRS)

|Dataset          |Symptom            |Device           |Sensor         |Device location                  |Subjects        |
|-----------------|-------------------|-----------------|---------------|---------------------------------|----------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|Tremor, gait, and other motor symptoms|MC10 BioStamp RC|Accelerometer|Trunk, left thigh, right thigh, left forearm, right forearm| 17 HC and 17 PD|
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)                                                                    |FoG    |                |             |                                                           |                | 
|REMPARK- nota: tem que se pedir acesso ao dataset                          |       |                |             |                                                           |                |
|PhysioNet                         |       |                |             |                                                           |                |
|Parkinsons Data Set (Oxford)      |       |                |             |                                                           |                |
|Parkinsons Telemonitoring         |       |                |             |                                                           |                |
|Parkinson Speech data set         |       |                |             |                                                           |                |
|Parkinson's Disease Classification|       |                |             |                                                           |                |
|mPower                            |       |                |             |                                                           |                |
|MJFF Levodopa Response Study      |       |                |             |                                                           |                |
|CuPID                             |       |                |             |                                                           |                |

|Dataset                                                                                                                                       |Year of creation|Language|Size    |File format(s)|Availability|
|----------------------------------------------------------------------------------------------------------------------------------------------|----------------|--------|--------|--------------|------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|2021            |English |10.76 GB|.csv          |Public      |
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)                                                                   |                |        |    |              | 
|REMPARK- nota: tem que se pedir acesso ao dataset                                                                                             |                |        |    |              |
|PhysioNet                         |       |                |             |                                                           |                |
|Parkinsons Data Set (Oxford)      |       |                |             |                                                           |                |
|Parkinsons Telemonitoring         |       |                |             |                                                           |                |
|Parkinson Speech data set         |       |                |             |                                                           |                |
|Parkinson's Disease Classification|       |                |             |                                                           |                |
|mPower                            |       |                |             |                                                           |                |
|MJFF Levodopa Response Study      |       |                |             |                                                           |                |
|CuPID                             |       |                |             |                                                           |                |

## PD-BioStampRC
Year of creation: 2021 (Last update in 2022)

Dataset: https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0

Cite: [Adams JL, Dinesh K, Snyder CW, Xiong M, Tarolli CG, Sharma S, Dorsey E, Sharma G. "A real-world study of wearable sensors in Parkinson’s disease". NPJ Parkinson's disease. 2021 Nov 29;7(1):1-8.](https://www.nature.com/articles/s41531-021-00248-w)

### Description

This dataset provides accelerometer data for studying activity, gait, tremor, and other motor symptoms in individuals wih PD. It also includes data from a healthy control group collected during the same collection protocol. The data collection started during a clinical evaluation using the UPDRS and was conducted for around two days afterwards in free-living conditions.

This dataset contains sensore, UDRS-assessment-annotation data, and demographic and clinical assessment data.

- Accelerometer sensor data: files corresponding to each sensor location for each patient, with each file containing a timestamp for each measurement and the corresponding acceleration values for each axis of the sensor;
- Annotation file: Contains annotations of the duration of various clinical assessments, through the start and end timestamps, the body location of the seessment, and the medication status;
- Demographic and clinical assessment data: Contains demographic data and the scores for the rest tremor amplitude on the right and left upper and lower extremities during the ON and OFF medication states.

Units: The accelerations is in g and the timstamps are in miliseconds and start counting from the from the instant of the earliest sensor recording.


## Daphnet

Dataset: https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait
