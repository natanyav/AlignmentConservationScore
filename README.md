# AlignmentConservationScore



AlignmentConservationScore is a program written in Python 3. The user can input amino acid sequences, perform multiple sequence comparison by log expectation (MUSCLE), and calculate the conservation score and sequence logo via WebLogo3 all in the same code. Perform the following steps to use the code.

  - Download .fasta files from UniProt and add them to your working directory
  - Install the following packages so that the program runs properly:
````
Biopython 1.77
MUSCLE (muscle3.8.31_i86win32.exe)
WebLogo 3
Ghostscript API (gs952w64.exe)
````

  - Enter the names of your input and output fasta files (.fas) in the MUSCLE wrapper. You will get an output string.
  - Convert output string into a handle and align your sequences. Note that this format of MUSCLE has difficulty aligning files that contain over 50 sequences.
  - Input your aligned file to WebLogo API. Keep in mind that the output is in eps byte array as a default.
  - Convert your eps byte array to a png image by using the png_print_formatter function which utilizes Ghostscript API to translate eps to png. 
  - The .png image will show a sequence logo and conservation scores based on your alignment. 


### Download packages
AlignmentConservationScore requires the following packages and libraries:

* [Biopython] - Free tools for biological applications
* [MUSCLE] - multiple sequence comparison by log expectation (MUSCLE)
* [WebLogo] - calculate the conservation score and sequence logo of aligned sequnces
* [Ghostscript] - translates eps format to png and jpeg


   [Biopython]: <https://biopython.org/>
   [MUSCLE]: <https://www.drive5.com/muscle/downloads.htm>
   [WebLogo]: <http://weblogo.threeplusone.com/>
   [Ghostscript]: <https://www.ghostscript.com/>
 
