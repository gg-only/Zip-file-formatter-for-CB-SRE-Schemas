# Zip-file-formatter-for-CB-SRE-Schemas

***Overview***

This is a public utility that helps users generate CB-compatible schema ZIP files from JSON definitions.

The tool allows you to upload a JSON file (for SRE EF or AS), formats it into the required ZIP structure, and produces a file that can be directly imported into a CB instance to register the schema.

Anyone can download and use this tool.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------
***How to Use***

1. Download the schema_gen.html file from this repository.

2. Open the file in any modern web browser (Chrome, Edge, Firefox, etc.).

3. On opening the page, you will be prompted to upload a file.

4. Upload a valid .json file.

---
***The tool will:***

1. Validate and format the JSON

2. Automatically generate a CB-compatible ZIP file

3. Auto-download the ZIP file to your system

4. Upload the generated ZIP file directly into your CB instance to make the schema live.
-------

***Supported Use Cases***

1. SRE EF schemas

2. SRE AS schemas

------
***Limitations & Important Notes***

1. This tool only supports SRE EF and AS schemas.

2. The uploaded file must be a valid .json file:

    -Downloaded from GitHub (respective branches), or

    -Manually prepared following the expected schema format.

    -Do not keep duplicate ZIP files with the same name in your system:

     If a ZIP with the same name already exists, the OS will auto-rename the new file (e.g., schema(1).zip, schema(2).zip). CB will reject renamed ZIP files, and schema import will fail
      Fix by either:

      -Deleting the duplicate ZIP files, or

      -Moving the new ZIP to a clean folder and renaming it correctly

      -Do NOT rename the ZIP file:
      
--------
***ZIP name format:***

schema_<EF_or_AS_name>.zip


***Note:*** CB follows strict naming conventions, and renaming the file will cause import failures.
