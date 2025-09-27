\# Neuroscience Data Structure (NDS)



The objective of this project is to put together a set of specifications and tools that would allow the standardization of a directory structure containing experimental data recorded with animal models in neuroscience.  

For this, we aim at capitalizing on the success of BIDS for human neuroimaging data, while retaining the specificities of data sets obtained in animal models.  

Such a standardized data structure will facilitate obtaining reproducible research and data sharing following the FAIR principles.  

\[Note that the name Neuroscience Data Structure and the associated acronym NDS are purely provisional.]



---



\## Examples



Here’s a minimal example of how to organize subject and session data in NDS:



```json

{

&nbsp; "subject": {

&nbsp;   "id": "sub-001",

&nbsp;   "species": "Mus musculus",

&nbsp;   "age": 12,

&nbsp;   "sex": "F"

&nbsp; },

&nbsp; "session": {

&nbsp;   "id": "ses-001",

&nbsp;   "task": "visual\_stimulus",

&nbsp;   "acquisition": {

&nbsp;     "device": "EEG",

&nbsp;     "channels": 64

&nbsp;   }

&nbsp; }

}



