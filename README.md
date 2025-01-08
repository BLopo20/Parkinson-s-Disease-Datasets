# Parkinson-Disease-Datasets

This repository contains datasets collected using sensor devices or microphones that can be used for the evaluation of Parkinson's disease (PD) motor symptoms or voice. This repository contains two main table describing characteristics of the datasets, the first containing information about the collection of the data and the other containing information like the size, language, and year of creation of the datasets. After these tables, the datasets are explored in more detail.

Unified Parkinson's Disease Rating Scale (UPDRS)

|Dataset          |Symptom            |Sensor         |Device location                  |Subjects        |
|-----------------|-------------------|---------------|---------------------------------|----------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|Tremor, gait, and other motor symptoms|Acc|Trunk, both thighs, both forearms| 17 HC and 17 PD|
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)|FoG|Acc|Hip, ankle, and upper leg|10 PD|
|[Oday](https://github.com/stanfordnmbl/imu-fog-detection/tree/main)|FoG|Acc and Gyro|Both feet, both ankles, both wrists,both thigs, lumbar, chest, and head|7 PD|
|[PADS](https://physionet.org/content/parkinsons-disease-smartwatch/1.0.0/#files-panel)|Tremor|Acc and Gyro|Both wrists|276 PD, 79 HC, and 114 DD|
|[MJFF Levodopa Response Study](https://www.synapse.org/Synapse:syn20681023/wiki/594680)|Motor fluctuations|Acc|Both wrists, both ankles, and waist|31 PD|
|[mPower](https://www.synapse.org/Synapse:syn4993293/wiki/247859)|Spatial memory, voice changes, gait, balance, and other motor symptoms|Acc, Gyro, magnetometer, pedometer, and microphone|N/A|9520|
|Parkinsons Data Set (Oxford)      |       |             |                                                           |                |
|Parkinsons Telemonitoring         |       |             |                                                           |                |
|Parkinson Speech data set         |       |             |                                                           |                |
|Parkinson's Disease Classification|       |             |                                                           |                |



|Dataset                                                                                                                                       |Year|Language|File format(s)                  |Availability|
|----------------------------------------------------------------------------------------------------------------------------------------------|----|--------|--------------------------------|------------|
|[PD-BioStampRC21](https://ieee-dataport.org/open-access/pd-biostamprc21-parkinsons-disease-accelerometry-dataset-five-wearable-sensor-study-0)|2021|English |.csv                            |Public      |
|[Daphnet](https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait)                                                                   |2013|English |.txt                            |Public      |
|[Oday](https://github.com/stanfordnmbl/imu-fog-detection/tree/main)                                                                           |2021|English |.xslx                           |Public      |
|[PADS](https://physionet.org/content/parkinsons-disease-smartwatch/1.0.0/#files-panel)                                                        |2024|English |.json, .txt, .py, .bin, and .csv|Public      |
|[MJFF Levodopa Response Study](https://www.synapse.org/Synapse:syn20681023/wiki/594680)                                                       |2019|English |.txt                            |Private     |
|[mPower](https://www.synapse.org/Synapse:syn4993293/wiki/247859)                                                                              |2015|English |.json and .m4a                  |Private     |
|Parkinsons Data Set (Oxford)                                                                                                                  |    |        |                                |            |
|Parkinsons Telemonitoring                                                                                                                     |    |        |                                |            |
|Parkinson Speech data set                                                                                                                     |    |        |                                |            |
|Parkinson's Disease Classification                                                                                                            |    |        |                                |            |


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

Note: 
- The dataset has a sampling frequency of 31.25 Hz.
- Despite authors mentioning this dataset can be used to study activity, gait, tremor and other motor siymptoms, only the clinical assessment data for rest tremor is available. The mean values for other test are show in the paper, however the values for wach individual subject are not disclosed.

## Daphnet

Dataset: https://archive.ics.uci.edu/dataset/245/daphnet+freezing+of+gait

Publication: [Bachlin, M., Plotnik, M., Roggen, D., Maidan, I., Hausdorff, J. M., Giladi, N., & Troster, G. (2009). Wearable assistant for Parkinson’s disease patients with the freezing of gait symptom. IEEE Transactions on Information Technology in Biomedicine, 14(2), 436-446.](https://ieeexplore.ieee.org/abstract/document/5325884)

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

Note: 
- Two patients (ID 02 and ID 08) reported fequent FOG episodes during the ON medication state and, consequently, performed the data collection on the ON state. 

## Oday

Dataset: https://github.com/stanfordnmbl/imu-fog-detection/tree/main

Publication: [O’Day, J., Lee, M., Seagers, K. et al. Assessing inertial measurement unit locations for freezing of gait detection and patient preference. J NeuroEngineering Rehabil 19, 20 (2022). https://doi.org/10.1186/s12984-022-00992-x](https://jneuroengrehab.biomedcentral.com/articles/10.1186/s12984-022-00992-x)

### Description

This dataset provides accelerometer and gyroscope data for the detection of FoG. The data was collected while the subjects walked independently through a turning and barier course, designed to elicit FoG, while wearing the inertial measuring units (IMUs).

Each walking trial consisted of two elipses and two figures of eight around tall barriers. Each subject performed 5 to 14 walking trials trough 2 to 6 visits, separated by up to 44 months. The walking trials were completed while the subjects were on the OFF medication status and off deep brain stimulation (DBS).

From the 7 subjects, 4 wore 11 IMUs placed on the locations described in the first table in the begining of the repository (both feet, booth ankles , both wrists, both thighs, lumbar, chest, and head) and the remaining 3 subjects wore only 6 IMUs placed on both feet, both ankles, lumbar, and chest. The subjects demographic data is shown in the following table. 

|Characteristic                               |PD group (n=7)|
|---------------------------------------------|--------------|
|Age                                          |51 - 68       |
|Sex (Male/Female)                            |4/3           |
|Disease duratuion                            |5 - 15        |
|Nº of walks (total of all subjects)          |60            |
|% time FoG (mena across walks)               |19.7 ± 19.9   |
|Nº FoG events (mean across walks)            |3.5 ± 3.1     |

Each dafa file corresponds to a walking task of a subject and contains, in each sample, the time, the accelerometer and gyroscope values of each of the X, Y, and Z axes for every IMU the patient wore, and the FoG label. This label can be 0 for non FoG or 1 for FoG. To obtain the FoG label, a video of each walking task was synchronized with the IMU system and an experienced rater identified the start and end times of FoG events in the video recordings.

Units: The acceleration is in m/s², the gyroscope is in rad/s and the time is in seconds.

Note:
- The dataset has a sampling frequency of 128 Hz.
- The dataset also contains code to pre-process, train, and evaluate convolutional neural networks that identify FoG.

## PADS - Parkinson's Disease Smartwatch dataset

Dataset: https://physionet.org/content/parkinsons-disease-smartwatch/1.0.0/#files-panel

Publication: [Varghese, J., Brenner, A., Fujarski, M., van Alen, C.M., Plagwitz, L., & Warnecke, T. (2024). Machine Learning in the Parkinson's disease smartwatch (PADS) dataset. npj Parkinsons Dis. 10, 9.](https://www.nature.com/articles/s41531-023-00625-7)

### Description

This dataset provides accelerometer and gyroscope data collected using two smartwatches during clinical assessment of PD paatients, patients with other similar movement disorders and healthy controls. The data acquisition was divided into the completion of eletronic questionnaires and the active movemet assessment. For the active movement assessment the subjects wore the two smartwatches on their wrists and the sensors recorded data during the performance of 11 movement tasks desiged to provoke subtel changes in movement pathologies and triger tremor characteristics. Each of the following tasks was performed for 10 to 20 seconds depending on the task and is associated with a particular ype of tremor:
- Resting with closed eyes while sitting (20 seconds) - resting tremor;
- Resting while patient is calculating serial sevens (20 seconds) - resting tremor;
- Lift and extend arms (10 seconds) - postural tremor;
- Remain arms lifted (10 seconds) - postural tremor;
- Hold 1 kg weight in each hand for 5 seconds - postural tremor;
- Point index finger to the examiners lifted hand (10 seconds) - kinetic tremor;
- Drink from glass (10 seconds) - kinetic tremor;
- Cross and extend both arms (10 seconds) - kinetic tremor;
- Bring both index fingers to each other (10 seconds);
- Tap own nose with index finger (10 seconds) - inetis tremor;
- Stomp on the ground while having the arms extended (20 seconds) - postural tremor.

The differential diagnosis (DD) group includes subjects with Atypical Parkinsonism, Essential Tremor, Multiple Sclerosis, or other movement disorders. The demographic data of the three groups of subjects is shown in the following table.

|Characteristic   |PD group (n=276)|HC group (n=79)|DD group (n=114)|
|-----------------|----------------|---------------|----------------|
|Age              |65.4 ± 9.6      |62.9 ± 12.5    |62.4 ± 11.5     |
|Sex (Male/Female)|195/81          |29/50          |57/57           |
|Age at diagnosis |58.26 ± 10.62   |N/A            |52.96 ± 16.52   |

The following table contains the folders in the dataset, an example of the name and type of files in each folder and a description of each file.

|Folders      |Files name and type                                 |Description                                             |
|-------------|----------------------------------------------------|--------------------------------------------------------|
|movement     |observation_001.json and 001_CrossArms_LeftWrist.txt|The .json file holds all meta information. The .txt files are in a separate folder called timeseries and hold the smartwatch records.| 
|questionaires|questionnaire_response_001.json                     |This file holds the questionnaire data.|
|patients     |patient_001.json                                    |This file holds all relevant metadata of the patient.|
|scripts      |run_preprocessing.py                                |This file holds exemplary coda that shows how data can be accessed usin Python.|
|preprocessed |001_ml.bin, 001_ml.bin, and file_list.csv           |This file holds the pre-processed files, in two separate files called movement and questionnaire, and a .csv file that gives an overview of all samples.|

Units: The acceleration is in g and the gyroscope is in rad/s.

Note:
- The dataset has a sampling frequency of 100 Hz.

## MJFF Levedopa Response Study

Dataset: https://www.synapse.org/Synapse:syn20681023/wiki/

Publication: 
[Daneault, JF., Vergara-Diaz, G., Parisi, F. et al. Accelerometer data collected with a minimum set of wearable sensors from subjects with Parkinson’s disease. Sci Data 8, 48 (2021). https://doi.org/10.1038/s41597-021-00830-0](https://www.nature.com/articles/s41597-021-00830-0)

[Vergara-Diaz, G., Daneault, JF., Parisi, F. et al. Limb and trunk accelerometer data collected with wearable sensors from subjects with Parkinson’s disease. Sci Data 8, 47 (2021). https://doi.org/10.1038/s41597-021-00831-z](https://www.nature.com/articles/s41597-021-00831-z)

## Description

This dataset provides data from 3 or 8 sensors collected both in clinical and home settings to evaluate wheter mobile sensors can be used to track motor fluctuations caused by Levodopa treatment. These motor fluctuations include dyskinesia and depleting effectiveness at controlling symptoms.

All study participants wore at least 3 sensors, a GeneActiv on the wrist of the most affected limb, a Pebble smartwatch on the wrist of the least affected limb, and a Samsung Galaxy Mini smartphone in a fanny pack worn in front of the waist. Of the 31 subjects, 19 also wore 5 Shimmer 3 sensors placed, with one of these sesors placed on each limb and on placed on the lower back. Subjects that wore the Shimmer 3 sensor performed a slightly expanded protocol.

Data was collected on 4 days. On the first day, subjects were on the ON medication state and performed section III of the MDS-UPDRS in the lab. Afterwards, subjects performed several motor tasks, listed bellow. The performance of these tasks was repeated 6 to 8 times at 30 minute intervals. A clinician provided labels of symptom severity and/or presence for each task.
- Standing;
- Walking in a straight line for 30s;
- Walking in a straight line for 30s while counting backwards;
- Walking upstairs and down stairs;
- Walking through a narrow corridor;
- Finger-to-nose for 15s (twice with each arm);
- Alternating hand movements for 15s (twice with each arm);
- Drawing;
- Typing on a keyboard for 30s;
- Opening a bottle and pouring water (three times);
- Arranging sheets of paper in a folder (twice);
- Assembling nuts and bolts for 30s;
- Folding a towel three times;
- Sitting.

After the data collection on the first day, subjects were sent home wearing the sensors and were instructed to conduct their usual activities for the following two days, recording medication intake and doses and the time they went to sleep and woke up. Furthermore, subjects that wore the Shimmer sensor were asked to performe motor tasks corresponding to specific item of section III of the MDS-UPDRS every 30 minutes for a total of 7 times each day.

On the fourth day, patients came back to the lab on the OFF medication state and repeated the procedure that was performed on the first day. However, the first time subjects performed the motor tasks was on the OFF state and the following repetitions were on the ON state.

Units: The acceleration is in m/s².

Note: 
- The dataset has a sampling frequency of 50 Hz.
- Data from two subjects were excluded  because some of the motor tasks were modified according to issues encountered during the first assessment. Data from another subject was excluded due to a technical malfunction of the sensors that lead to a substancial amount of missing data.
- Subject 11_NYC swapped the positions of the GENEActiv and Pebble devices after the first session in the lab, on the first day. For this subject that session ended at the timestamp 1433495025.7.

## How to access the data

The dataset is available in the Synapse platform. To access the dataset researchers can follow the steps bellow:
1. Register for a Synapse account;
2. Become a certified Synapse user;
3. Have your user profile validated;
4. Request access to the data and submit your intended data use statement;
5. Agree to the data-specific conditions of use;
6. Download the data.

These steps are explained more indept in the "Accessing the Data" section of dataset link.

## mPower

Dataset: https://www.synapse.org/Synapse:syn4993293/wiki/247859

Publication: [Bot, B., Suver, C., Neto, E. et al. The mPower study, Parkinson disease mobile data collected using ResearchKit. Sci Data 3, 160011 (2016). https://doi.org/10.1038/sdata.2016.11](https://www.nature.com/articles/sdata201611)

### Description

This database is based on a mobile application study that supplements traditional symptom measurements with metrics collected using the sensors in mobile devices. The Parkinson mPower app allowed the survey of a large, longitudinal cohort of volunteers with PD and healthy controls.

The dataset contains data from the following seven study tasks:
- Demographic: subjects respond to questions about general demographic topics and health history;
- MDS-UPDRS: subjects respond to selected questions from the MDS-UPDRS scale;
- PDQ-8: subjects reespond to a short form of a Parkinson's Disease Questionnaire;
- Memory: subjects complete a short visuospatial game related to the Corsi block tapping test;
- Tapping: subjects repeatedly tap their phone's screen;
- Voice: subjects record ambient noise lever for 5 seconds and, if the noise level is acceptable, record themselves saying "aaah" for 10 seconds;
- Walking: subjects walk back and forth for 20 to 30 seconds with their smartphones in their pocket and, afterwards, stand still for another 20 to 30 seconds;

The fisrt task is completed once when the subject first uses the app, the next two tasks are completed once a month, and the remaining tasks are completed three times a day. Subjects that self-identified as having a professional PD diagnosis were asked two performe the last four tasks immediatly before taking their medication, after taking their medication and at some other time. Subjects who did not self-identify has having a professional PD diagnosis could complete these tasks at any time during the day. 

For the walking task, data is collected from accelerometer, pedometer and core motion readings, which include attitude, rotation rate, acceleration, gravity, and magnetic field.

The mPower app was made available through the Apple App Store only in the United States. Enrollment was open to individuals diagnosed with PD and anyone that wanted to participate as a healthy control. A total of 9,520 subjects consented to the study and agreed to share their data. Of these, 8,320 completed at least one survey or task. Of the 6,805 who completed the enrollment survey, 1,087 self-identified as having a professional diagnosis of PD and 5,581 did not, with 137 opting not to answer the question. Despite follow up being nonuniform across participants, due to the nature of the study, 898 participants collected data at least five separate days over the course of the first six months. 

Units: The acceleration is in m/s².

## How to access the data

The dataset is available in the Synapse platform. To access the dataset researchers can follow the steps bellow:
1. Register for a Synapse account;
2. Become a certified Synapse user;
3. Have your user profile validated;
4. Request access to mPower Data and submit your intended data use statement;
5. Agree to the data-specific conditions of use;
6. Download the data.

Due to copyright restrictions associated with the MDS-UPDRS and PDQ-8 surveys, adittional steps are necessary to access MDS-UPDRS survey and PDQ-8 survey sensor data.

These steps are explained more indept in the "Accessing the Data" section of dataset link.

