# Parkinson-Disease-Datasets

This repository contains datasets collected using sensor devices or microphones that can be used for the evaluation of Parkinson's disease (PD) motor symptoms or voice. This repository contains two main table describing characteristics of the datasets, the first containing information about the collection of the data and the other containing information like the size, language, and year of creation of the datasets. After these tables, the datasets are explored in more detail.

Unified Parkinson's Disease Rating Scale (UPDRS)

|Dataset          |Symptom            |Sensor         |Device location                  |Subjects        |
|-----------------|-------------------|---------------|---------------------------------|----------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|Tremor, gait, and other motor symptoms|Accelerometer|Trunk, left thigh, right thigh, left forearm, right forearm| 17 HC and 17 PD|
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)                                                                    |Freezing of Gait (FoG)               |Accelerometer|Hip, ankle, and upper leg                                      |10 PD           | 
|PhysioNet                         |       |             |                                                           |                |
|Parkinsons Data Set (Oxford)      |       |             |                                                           |                |
|Parkinsons Telemonitoring         |       |             |                                                           |                |
|Parkinson Speech data set         |       |             |                                                           |                |
|Parkinson's Disease Classification|       |             |                                                           |                |
|mPower                            |       |             |                                                           |                |
|MJFF Levodopa Response Study      |       |             |                                                           |                |
|CuPID                             |       |             |                                                           |                |

|Dataset                                                                                                                                       |Year|Language|Size    |File format(s)|Availability|
|----------------------------------------------------------------------------------------------------------------------------------------------|----|--------|--------|--------------|------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|2021|English |10.76 GB|.csv          |Public      |
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)                                                                   |2013|English |20.5 MB |.txt          |Public      |
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

This dataset provides accelerometer data, collected using the MC BioStamp RC, for studying activity, gait, tremor, and other motor symptoms in individuals wih PD. It also includes data from a healthy control (HC) group collected during the same collection protocol. The data collection started during a clinical evaluation using the UPDRS and was conducted for around two days afterwards in free-living conditions.

The demografic data of the subjects from both groups are shown in the following table.

|Characteristic                                                       |PD group (n=17)|HC group (n=17)|
|---------------------------------------------------------------------|------------------|------------|
|Age                                                                  |66.4 ± 11.3       |64.0 ± 9.9  |
|Sex (women %)                                                        |41.2              |76.5        |
|Hoehn & Yahr stage                                                   |1.9 ± 0.8         |N/A         |
|Years since diagnosis                                                |4.8 ± 4.0         |N/A         |
|MDS-UPDRS - total rest treor score (mean ± standard deviation, range)|2.0 ± 1.6, 0.0-4.0|N/A         |
|MDS-UPDRS - total motor score (mean ± standard deviation)            |20.9 ± 7.9        |2.2 ± 2.1   |
|Timed Up and Go (mean ± standard deviation s)                        |10.4 ± 2.6        |8.4 ± 1.1   |
|10-m Walk Test (mean ± standard deviation s)                         |4.7 ± 1.1         |4.1 ± 0.5   | 

This dataset contains sensor data, UDRS-assessment-annotation data, and demographic and clinical assessment data.

- Accelerometer sensor data: files corresponding to each sensor location for each patient, with each file containing a timestamp for each measurement and the corresponding acceleration values for each axis of the sensor;
- Annotation file: Contains annotations of the duration of various clinical assessments, through the start and end timestamps, the body location of the seessment, and the medication status;
- Demographic and clinical assessment data: Contains demographic data and the scores for the rest tremor amplitude on the right and left upper and lower extremities during the ON and OFF medication states.

Units: The accelerations is in g and the timstamps are in miliseconds and start counting from the from the instant of the earliest sensor recording.

Note: Despite authors mentioning this dataset can be used to study activity, gait, tremor and other motor siymptoms, only the clinical assessment data for rest tremor is available. The mean values for other test are show in the paper, however the values for wach individual subject are not disclosed.


## Daphnet

Dataset: https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait

Cite: [Bachlin, M., Plotnik, M., Roggen, D., Maidan, I., Hausdorff, J. M., Giladi, N., & Troster, G. (2009). Wearable assistant for Parkinson’s disease patients with the freezing of gait symptom. IEEE Transactions on Information Technology in Biomedicine, 14(2), 436-446.](https://ieeexplore.ieee.org/abstract/document/5325884)

### Description

This dataset provides accelerometer data, collected with en emphasis on generating freeze events, to recognize gait freeze. The data was collected in the laboratory with accelerometers placed just above the ankle, on the upper leg above te knee, and on the lower belt (hip). Patients performed the data collection during the OFF mediacation state, in the morning. Data was collected during two sessions, each of about 10 to 15 minutes, while the users performed three tasks:
- Walking in a straight line;
- Random walking with numerous turns and initiated stops;
- Activities of daily living (ADL) tasks, where users went into different rooms while fetching coffe, opening doors, etc.

For the first session the devices recorded all necessary data during the performance of the tasks. The second session was a repetition of the first but with rythmic auditory stimulation (RAS) feedback activated. RAS was shown to be effective at improving gait of PD patients and for this collection was only used during an actual or impeding freezing of gait (FOG) event.

The data was collected from 10 idiophatic PD patients with a history of FOG that were able to walk unassisted during the OFF medication period. The demographic data of the subjects is shown in the following table.

|Characteristic                               |PD group (n=10)|
|---------------------------------------------|---------------|
|Age                                          |66.5 ± 4.8     |
|Sex (Male/Female)                            |7/3            |
|Disease duratuion                            |13.7 ± 9.67    |
|Hoehn & Yahr stage in the ON medication state|2.6 ± 0.65     |

Each file in the dataset contains a time sample and the corresponding sample data for the ankle acceleration, upper leg acceleration, and hip acceleration, with values for the horizontal forward, vertical, and horizontal lateral accelerations for each. Lastly, each file contains an annotation of 0, 1, or 2, where:
- 0: Sample is not part of the experiment (sensors are installed on the user or the user is performing activities unrelated to the experience);
- 1: No freeze (during the experiment, while patients can be standing, walking, or turning);
- 2: Freeze.

The annotations were obtaine by synchronizing the leg movement data with video recordings of the walking trials and having a physiotherapist take notes of relevant events during the sessions and identifying the start time, duration, and end time of freezing events. Moreover an assistant annotated the patients activity (e.g. standing, walking, turning, or freezing) during the recording session.

Units: The acceleration is in mg and the time of sample is in miliseconds.

Note:  Two patients (ID 02 and ID 08) reported fequent FOG episodes during the ON medication state and, consequently, performed the data collection on the ON state. 
