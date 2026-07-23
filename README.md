# InterGenSynchrony Dataset

---

A longitudinal fNIRS hyperscanning dataset of same generation and intergenerational relationship
development and collaboration.

## Authors
- Ryssa Moffat (rmoffat@ethz.ch)
- Emily S. Cross (ecross@ethz.ch)

[Social Brain Sciences Lab](https://sbs.ethz.ch/), ETH Zurich

## Citation
Moffat, R., & Cross, E. S. (2026). *InterGenSynchrony Dataset* [Data set]. OpenNeuro. [https://openneuro.org/datasets/ds008192/](https://openneuro.org/datasets/ds008192/)


## Licence
The InterGenSynchrony Dataset is shared under a CC-BY 4.0 licence.

---

## Dataset Structure
To describe the content of `.csv` files, we provide an easy-to-read Data Dictionary, as well computer-readable `.json` files, which are named to match the relevant `.csv` files.

```

InterGenSynch
├── DataDictionary.html
├── dataset_description.json
├── participants.json
├── participants.tsv
├── README.html
├── README.md
├── sourcedata
|   ├── hyperscanning
|   │   ├── dyadList.csv
|   │   ├── dyadList.json
|   │   │
|   │   ├── behaviour
|   │   │   ├── codedbehaviour.json
|   │   │   ├── experimenterratings.json
|   │   │   ├── sub-all_ses-all_codedbehaviour.csv
|   │   │   └── sub-all_ses-all_experimenterratings.csv
|   │   │
|   │   ├── coordinates
|   │   │   ├── channelLengths.json
|   │   │   ├── distancesToRoi.json
|   │   │   ├── optodeCoordinates.json
|   │   │   ├── sub-101
|   │   │   │   ├── ses-01
|   │   │   │   │   ├── sub-101_ses-01_acq-dyad1001_channelLengths.csv
|   │   │   │   │   ├── sub-101_ses-01_acq-dyad1001_distancesToRoi.csv
|   │   │   │   │   └── sub-101_ses-01_acq-dyad1001_optodeCoordinates.csv
|   │   │   │   ├── ses-02
|   │   │   │   └── ...
|   │   │   ├── sub-102
|   │   │   └── ...
|   │   │
|   │   ├── drawings
|   │   │   ├── alone
|   │   │   │   ├── sub-101_ses-01_acq-dyad1001_task-drawingalone_artwork.tif
|   │   │   │   ├── sub-101_ses-02_acq-dyad1001_task-drawingalone_artwork.tif
|   │   │   │   └── ...
|   │   │   └── codrawing
|   │   │       ├── ses-01_acq-dyad1001_task-codrawing1_artwork.tif
|   │   │       ├── ses-01_acq-dyad1001_task-codrawing2_artwork.tif
|   │   │       └── ...
|   │   │
|   │   ├── mocap
|   │   │   ├── mocap_IDs.csv
|   │   │   ├── mocap.json
|   │   │   ├── mocap_IDs.json
|   │   │   ├── acq-dyad1001
|   │   │   │   ├── ses-01
|   │   │   │   │   ├── ses-01_acq-dyad1001_task-drawingalone_mocap.csv
|   │   │   │   │   ├── ses-01_acq-dyad1001_task-codrawing1_mocap.csv
|   │   │   │   │   ├── ses-01_acq-dyad1001_task-codrawing2_mocap.csv
|   │   │   │   │   └── ses-01_acq-dyad1001_task-collaborativetask_mocap.csv
|   │   │   │   ├── ses-02
|   │   │   │   └── ...
|   │   │   ├── acq-dyad1002
|   │   │   └── ...
|   │   │
|   │   ├── qualitative
|   │   │   ├── exitinterviews
|   │   │   │   ├── exitinterview_questions.json
|   │   │   │   ├── sub-101_ses-06_acq-dyad1001_exitinterview.txt
|   │   │   │   ├── sub-102_ses-06_acq-dyad1002_exitinterview.txt
|   │   │   │   └── ...
|   │   │   └── textcomments
|   │   │       ├── sub-all_ses-all_textcomments.csv
|   │   │       └── textcomments.json
|   │   │
|   │   └── selfreport
|   │       ├── pre-selfreport-raw.json
|   │       ├── post-selfreport-raw.json
|   │       ├── sub-all_ses-all_pre-selfreport-raw.csv
|   │       └── sub-all_ses-all_post-selfreport-raw.csv
|   │
|   └── ratings
|       ├── external_ratings_of_drawings.csv
|       └── external_ratings_of_drawings.json
│
├── sub-101
│   ├── ses-02
│   │   ├── nirs
│   │   │   ├── sub-101_ses-02_acq-dyad1001_coordsystem.json
│   │   │   ├── sub-101_ses-02_acq-dyad1001_optodes.tsv
│   │   │   ├── sub-101_ses-02_task-drawing_acq-dyad1001_run-01_channels.tsv
│   │   │   ├── sub-101_ses-02_task-drawing_acq-dyad1001_run-01_events.json
│   │   │   ├── sub-101_ses-02_task-drawing_acq-dyad1001_run-01_events.tsv
│   │   │   ├── sub-101_ses-02_task-drawing_acq-dyad1001_run-01_nirs.json
│   │   │   └── sub-101_ses-02_task-drawing_acq-dyad1001_run-01_nirs.snirf
│   │   └── sub-101_ses-02_scans.tsv
│   ├── ses-03
│   └── ...
├── sub-102
└── ...

```




---

## Participants

*Main hyperscanning experiment:* Participants include 122 community-dwelling adults from Zurich, Switzerland. Of these, 31 were older adults (aged 69+ years) and 91 were younger adults (aged 18–35 years). Participants were assigned to intergenerational dyads (n = 31) and same generation dyads (n = 30) based on availability for sessions (e.g., matching people available at the same day/time for 6 consecutive weeks). 

*External rating of drawings:* External raters, recruited via Prolific, were 103 residents of the United Kingdom, who were 18 years of age or above, proficient English speakers, who had previously completed a minimum of 50 tasks on Prolific with a 100% approval rate.

---

## Data Modalities

The dataset is divided into two parts.

The root folder contains the fNIRS recordings from the main longitudinal hyperscanning experiment.

Inside the `sourcedata/` folder, the `hyperscanning/` folder contains the other data modalities from the main longitudinal hyperscanning experiment. The `ratings/` folder contains external raters' ratings of the drawings produced in the main experiment.

### Root folder
#### fNIRS
Inside the root folder, the fNIRS data are organised according to BIDS conventions. This includes a folder per participant (e.g., `sub-101/`) that contains a folder for each session (e.g., `ses-02/`). The `ses-XX/` folder contains a file listing recordings (`*_scans.tsv`) and a `nirs/` folder with:

- raw fNIRS recordings (`*_nirs.snirf`)
- device and recording information (`*_nirs.json`)
- event (trigger) information (`*_events.tsv`)
- channel information, including channels identified as having no cardiac oscillation by visual inspection (`*_channels.tsv`)
- optode montage information in channel-space (`*_optodes.tsv`)
- MNI coordinate system information (`*_coordsystem.json`)

### Sourcedata
#### Hyperscanning
##### Behaviour

`behaviour/` contains

- scored behaviour during collaborative tasks (`sub-all_ses-all_codedbehaviour.csv`)
- experimenter ratings of simultaneous drawing behaviour (`sub-all_ses-all_experimenterratings.csv`)

##### Coordinates

`coordinates/` contains a folder per participant with a subfolder per session (`sub-XXX/ses-XX/`) that contains:

- digitised positions of optodes in MNI coordinates (`*_optodeCoordinates.csv`)
- the distance between source-detector pairs (`*_channelLengths.csv`)
- the distance from the centre of each channel to the centre of each region of interest (`*_distancesToRoi.csv`)

##### Drawings

`drawings/` contains two subfolders:

- `alone/` — images of drawings made by participants individually
- `codrawing/` — images of drawings made by dyads together

##### Motion Capture

`mocap/` contains a folder per dyad (e.g., `acq-dyad1001/`) with a subfolder per session (`ses-XX/`) that contains the 2D motion capture coordinates per drawing and collaborative activity separately.

##### Qualitative

`qualitative/` contains two subfolders:

- `exitinterviews/` — transcripts of exit interviews per participant
- `textcomments/` — text-based reflections from all participants in a single file (`sub-all_ses-all_textcomments.csv`)

##### Self-Report

`selfreport/` contains raw self-reported questionnaire responses recorded:

- before each session (`*_pre-selfreport-raw.csv`)
- after each session (`*_post-selfreport-raw.csv`).

#### Ratings

`ratings/` contains external raters' ratings of the co-drawn drawings produced in the main dataset.

---




