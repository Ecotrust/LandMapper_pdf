# LandMapper_pdf
Populating a pdf document with images and text using pdfjinja package. [Link to pdfjinja repository.](https://github.com/rammie/pdfjinja)

Be sure to check out installation and dependency information.

## Contents
* LM_populatePDF.ipynb - notebook containing the code that populates the template pdf  
* LM_form.pdf - pdf template  
* LMpdf_output.pdf - populated output pdf  
* img folder - .png files are images to be inserted  
* environment.yml - conda enviroment 

## Notes
* One of the dependencies of pdfjinja is [pdftk](https://www.pdflabs.com/tools/pdftk-server/) which must be installed, is that a barrier?
* This method requires an image stored to drive.  I didn't explore other possibilities (array, etc.).
* Not super quick, this small example took ~45 seconds.
* We would need to dynamically change text and image inputs based on selected property. 


