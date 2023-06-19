# Truecasing German ELSST terms
The ELSST Thesaurus terms are currently written in all caps but need to be transformed to regular German capitalization

## Files and folders
- The Jupyter notebook contains the code which runs on the test file (ELSST_R3_DE.xlsx). 
- The folder /wortliste/ contains the list of verbs and nouns.
- The folder /forELSSTGroup contains the output files of the different steps.

### Output files

- 'GER_ELSST_lowercase.xlsx' is everything converted to lowercase
- 'GER_ELSST_definitions.xlsx' has the first string of the notes and definitions capitalized (as these are full sentences rather than individual terms or phrases)
- 'GER_ELSST_targetfile1.xlsx': all strings in the nouns list and not in the verbs list are capitalized
- 'GER_ELSST_targetfile2.xlsx': all strings ending in -heit, -keit, -ung, etc. (which are always nouns) are capitalized
- 'GER_ELSST_targetfile3.xlsx': In this step, all strings are capitalized which end in a word from the list of nouns (and not in the list of verbs). As you can see this works fairly well for the labels, but produces many false-positives in the definitions and scope notes. For example 'politischen' is wrongly capitalized because it contains 'Tischen'. We should consider to exclude the notes and definitions in last step. 

## Binder notebook

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jonasre123/ELSST-Group.git/HEAD)
