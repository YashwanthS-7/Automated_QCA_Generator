Automated QCA Design using Yosys & MVSIS
This project aims to automate the generation of input files for the QCA LG Generator by leveraging Yosys and MVSIS for logic synthesis and optimization.

Current Progress & Workflow
Generating .lsi Files

Tools Used: Yosys (open-source alternative to Synopsys).
Challenges: Synopsys is commercial software with no student license.
Solution: Yosys synthesizes Verilog (.v) files and exports Netlists in .blif format.
Conversion: A Python-based converter transforms .v files from Yosys into .lsi format.
Generating .gate Files

Tools Used: MVSIS (successor: SIS).
Workflow:
Import .blif file from Yosys into MVSIS.
Generate .gate file.
Challenges: The qca.genlib library is outdated, causing issues in generating accurate .gate files.
Python Script Development

Developed a Python script to automate .lsi, .vhd, and .gate file generation.
Current Limitations:
Errors and inconsistencies in generated files.
Limited to single-gate equations.
Documentation & Installation

Created an instructional video covering Yosys & MVSIS installation and usage.
Next Steps
Resolving MVSIS compatibility issues.
Enhancing Python script to handle complex circuits.
Validating the generated files with QCA LG Generator.
