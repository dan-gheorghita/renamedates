# renameDates.py

**Python Script Analysis: RenameDates.py**

The `renameDates.py` script is a Python program designed to rename files in the current working directory that follow the American date format (`MM-DD-YYYY`) to the European date format (`DD-MM-YYYY`).

**Key Features:**

1. **Pattern Matching:** The script uses a regular expression (`regex`) to match filenames containing the American date format. The pattern is defined using a verbose syntax to ensure readability.
2. **File Looping:** The script iterates over the files in the current working directory using `os.listdir('.')`.
3. **Filename Parsing:** For each matched file, the script extracts the different parts of the filename using the matched groups of the regex pattern.
4. **European Filename Generation:** The script constructs the European-style filename by rearranging the extracted parts.
5. **File Renaming:** The script prints the renaming operation to the console and comments out the actual file renaming using `shutil.move()` to prevent