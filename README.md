# File Organizer – Internship Technical Challenge 2025

## Option Chosen
**Option 1 – File Organizer**

This program organizes files in a given folder into subfolders based on their file type.

--

## How to Run

### In Google Colab
1. Open the notebook `file_organizer.ipynb` in [Google Colab](https://colab.research.google.com/).
2. Run all cells in order.
3. Update the `folder` path in the test cell to point to the directory you want to organize (can be a local folder you upload to Colab, or a Google Drive folder you mount).
4. Run in **simulate mode** to preview:
   ```python
   organize_folder("path/to/folder", simulate=True)
5. Run without simulate=True to actually move files:
   ```python
   organize_folder("path/to/folder", simulate=False)

### Locally with Python
If you prefer, download the notebook as a Python script (.py) from Colab:
	•	File → Download → Download .py
	•	Then run in your terminal with Python 3.8+.
 
 --

## Language and Tools
### 1. Language: 
Python 3 (developed in Google Colab)
### 2. Tools:
	•	Google Colab (for development and testing)
	•	Standard Python library only (no external dependencies required)

--

## Extra Features (Bonus)
### 1. Simulation Mode (simulate=True): 
preview which files would be moved without making changes.
### 2. Summary Report: 
prints how many files were moved into each category.
### 3. Automatic Subfolder Creation: 
creates Images/, Documents/, Videos/, and Others/ folders if they do not exist.
### 4. Collision Handling: 
if a file with the same name already exists in the target folder, the script renames the new file with a timestamp to avoid overwriting.

--

## Notes
	•	Only scans the given folder (does not process subfolders).
	•	You can modify the EXT_MAP dictionary inside the function to support additional file types.
	•	The notebook was saved directly to GitHub (.ipynb format) to preserve the Colab workflow.

--

## Repository Structure
File-Organizer/
│
├── file_organizer.ipynb   # Main notebook with implementation and tests
└── README.md              # Project documentation

--

## Example Output

### 1. Simulate Mode

[SIMULATE] Would move: photo.jpg → Images/
[SIMULATE] Would move: doc.pdf → Documents/
[SIMULATE] Would move: video.mp4 → Videos/
[SIMULATE] Would move: notes.txt → Documents/
[SIMULATE] Would move: audio.mp3 → Others/

### 2. Organize Mode

Moved: photo.jpg → Images/
Moved: doc.pdf → Documents/
Moved: video.mp4 → Videos/
Moved: notes.txt → Documents/
Moved: audio.mp3 → Others/

Summary:
  Documents: 2
  Images: 1
  Others: 1
  Videos: 1
Total files moved: 5
