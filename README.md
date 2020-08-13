# LandMapper_pdf
Populating a pdf document with images and text using pdfjinja package. [Link to pdfjinja repository.](https://github.com/rammie/pdfjinja)

Be sure to check out installation and dependency information.

## Dependencies
[pdftk server](https://www.pdflabs.com/tools/pdftk-server/)
Ubuntu - not available using pip. use snap instead and then create a symlink.
  * install with snap
    `sudo snap install pdftk`
  * create a symlink
    `sudo ln -s /snap/pdftk/current/usr/bin/pdftk /usr/bin/pdftk`

## Troubleshooting
```
  Error: Unable to find file
  Error: Unable to find file.
  Error: Failed to open PDF file:
  input.pdf
  Errors encountered. No output created.
  Done. Input errors, so no output created.
```
* install pdftk using snap and create a symlink
```
sudo snap install pdftk
sudo ln -s /snap/pdftk/current/usr/bin/pdftk /usr/bin/pdftk
```

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
