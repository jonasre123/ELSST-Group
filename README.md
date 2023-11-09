# Truecasing German ELSST terms
The ELSST Thesaurus terms are currently written in all caps but need to be transformed to regular German capitalization

## Files and folders
- The Jupyter notebook contains the code which runs on the test file (ELSST_R3_DE.xlsx). 
- The folder /wortliste/ contains the list of verbs and nouns.
- The folder /forELSSTGroup contains the output files of the different steps.

### Output files

- 'GER_ELSST_lowercase.xlsx' is everything converted to lowercase
- 'GER_ELSST_firstword.xlsx' has the first string character in all fields capitalized
- 'GER_ELSST_targetfile1.xlsx': all strings in the nouns list and not in the verbs list are capitalized
- 'GER_ELSST_targetfile2.xlsx': all strings ending in -heit, -keit, -ung, etc. (which are always nouns) are capitalized
- 'GER_ELSST_targetfile3.xlsx': The Hanover Tagger is used to identify additional nouns (esp. compounds) and capitalize them. 

## Binder notebook

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jonasre123/ELSST-Group.git/HEAD)
