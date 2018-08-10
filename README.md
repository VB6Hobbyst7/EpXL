# EpXL
A macro-enabled Microsoft Excel spreadsheet user-interface to the EnergyPlus™ whole-building energy simulation program (https://energyplus.net/). Developed as a result of frustration over the other user-interfaces, including the standard Energy Plus IDF editor, and overcomes the impossible task of editing .IDF text files directly. Will i future be converted to JSON output with the possibility for batch-automation for parametric studies.

### Functionality
- EpXL is distributed with the Input Data Dictionary (IDD) for Energy Plus v8.9.0. Whenever a new version of Energy Plus is relased, you can update EpXL by viewing sheet 'IDD', which automatically imports the latest data dictionary (.IDD file), or any earlier version of you choice. This process takes some time. Save the EpXL workbook after you have done this.
- Import EnergyPlus a Input Data File (.IDF) into EpXL by keying CTRL+I. Immediately after importing the file into sheet 'IDF', EpXL vets the data against the IDD, and comments all input values with popup comments. After this you can edit the data just like any spreadsheet by inserting or deleting rows and editing cells.
- At any time, you can vet the input data in sheet 'IDF' against the IDD by keying CTRL+Q (for Quality check). This also updates the popup comments.
- Viewing sheet 'Simulate' automatically runs EnergyPlus and shows a list of hyperlinks to important output files. 
- EpXL is written in Visual Basic for Applications (VBA), which you can be easily modify to automate your own simulation tasks.

### Summary of the main macros:
- CTRL+I: Import an .IDF file to sheet 'IDF'.
- CTRL+Q: Quality check of the input data in sheet 'IDF'.
- CTRL+E: Export the input data to a .IDF file. This is normally not necessary, as the 'Simulate' sheet does this anyway.
- Viewing the 'Simulate' sheet automatically exports .IDF, runs EnergyPlus, reports any errors, and compiles a hyperlink list of output files.
- Viewing the 'IDD' sheet automatically imports a .IDD data dictionary your choice. The latest dictionary is called "Energy+.idd" and is found in the EnergyPlus root directory on your PC.

### License & warranty
- Distributed under the GLP v3 lisence (https://www.gnu.org/licenses/gpl-3.0.en.html)
- Provided without warranty of any kind.

### Author & copyright
© Peter.Schild@OsloMet.no
