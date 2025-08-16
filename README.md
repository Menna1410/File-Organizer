# File Organizer – Internship Technical Challenge 2025

## Option Chosen
**Option 1 – File Organizer**

This program organizes files in a given folder into subfolders based on their file type.

---

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
