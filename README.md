# step2stl
utilizes FreeCAD's Python libraries to convert CAD files from STEP format to STL format.

This FreeCAD macro converts all STEP files located in a user-specified directory to STL format and writes the converted files to a user-specified output directory. It renames the files by replacing spaces with underscores for better compatibility with different systems.

To run this macro, you need FreeCAD installed on your machine.

## How to run the step2stl macro
1. Open FreeCAD GUI.
2. Go to Macro -> Macros....
3. Locate and select step2stl.FCMacro. Click on "Execute".
4. After executing the macro, you will be prompted to provide the following:

  * Input Directory: A directory containing the source .STEP files. All .STEP files in this directory will be processed.
  * Output Directory: The directory where the converted .STL files should be placed.

If the script encounters any issues while converting a file, it will continue to the next file and print an error message detailing the issue.

Please note that some limitations may apply to complex and large .step files, as their conversion is subject to FreeCAD's functionality and performance.

## Dependencies
*FreeCAD
* PySide for the GUI dialogs
