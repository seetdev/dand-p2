# Project Overview

- This project looks into analyzing a dataset that contains information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment.

- PatientId - Identification of a patient
- AppointmentID - Identification of each appointment
- Gender - Male or Female . Female is the greater proportion, woman takes way more care of they health in comparison to man.
- ScheduledDay - The day of the actual appointment, when they have to visit the doctor.
- AppointmentDay - The day someone called or registered the appointment, this is before appointment of course.
- Age - How old is the patient.
- Neighbourhood - Where the appointment takes place.
- Scholarship - True of False . Observation, this is a broad topic, consider reading this article https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia
- Hipertension - True or False
- Diabetes - True or False
- Alcoholism - True or False
- Handcap - True or False
- SMS_received - 1 or more messages sent to the patient.
- No-show - Be careful about the encoding of the last column: it says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.

## Analysis

The project will look into the following features and its impact on the No-Show behavior. The following questions can be tested against the dataset:

- Does Gender play a part in the show and no-show probability
- Does Age Group play a part in the show and no-show probability

## Directory Structure

This is the folder structure of the project

```bash
.
├── Investigate_a_Dataset.html                  ' Export of Jupyter Notebook run result in HTML
├── Investigate_a_Dataset.ipynb                 ' Jupyter Notebook code file
├── LICENSE                                     ' License File
├── PopulationAgeSex-20200531014022.xlsx        ' Age data obtained from UN
├── README.md                                   ' This file describing the project
├── dand.yml                                    ' Export of conda environment to run this notebook
└── noshowappointments-kagglev2-may-2016.zip    ' Compressed version of dataset source for project
```

## Setup

### Prerequisites

1. Python setup on the host
2. conda setup on the host
3. conda environment that is similar to dand.yml

### Running locally

1. Clone repository by running `git@github.com:seetdev/dand-p2.git`
2. Go into the cloned folder
3. Create conda environment `conda env create -f dand.yml`
4. Run the notebook using `jupyter notebook`