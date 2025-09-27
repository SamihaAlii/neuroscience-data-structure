# Minimal Neuroscience Data Structure (NDS) Example

This is a minimal example of how to organize subject and session data in NDS:

```json
{
  "subject": {
    "id": "sub-001",
    "species": "Mus musculus",
    "age": 12,
    "sex": "F"
  },
  "session": {
    "id": "ses-001",
    "task": "visual_stimulus",
    "acquisition": {
      "device": "EEG",
      "channels": 64
    }
  }
}
