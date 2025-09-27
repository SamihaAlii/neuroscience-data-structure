\# Neuroscience Data Structure (NDS) Examples



\## Raw vs Processed Data Example



In NDS, experimental data is organized into `raw/` and `processed/` directories:



project/

├── sub-001/

│ ├── ses-001/

│ │ ├── raw/

│ │ │ ├── eeg\_data.edf

│ │ │ └── video.mp4

│ │ └── processed/

│ │ ├── eeg\_cleaned.fif

│ │ └── motion\_tracking.csv



yaml

Copy code



\- `raw/`: contains the \*\*original unprocessed data\*\*.  

\- `processed/`: contains \*\*cleaned or analyzed data\*\*, ready for sharing or further analysis.



---



\## JSON Example for a Subject and Session



```json

{

&nbsp; "subject": {

&nbsp;   "id": "sub-002",

&nbsp;   "species": "Rattus norvegicus",

&nbsp;   "age": 20,

&nbsp;   "sex": "M"

&nbsp; },

&nbsp; "session": {

&nbsp;   "id": "ses-001",

&nbsp;   "task": "maze\_navigation",

&nbsp;   "acquisition": {

&nbsp;     "device": "VideoTracking",

&nbsp;     "frame\_rate": 30

&nbsp;   }

&nbsp; }

}

