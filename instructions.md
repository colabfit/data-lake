## Detailed Submission Instructions  
  
**Fill out and submit and issue**
  
* Click on `Issues` from the menu bar
* Click on `New issue`
* Select the `Dataset submission/request` template by clicking the `Get started` button
* Fill out the issue template, remembering to enter your dataset name in the issue title
* Submit the issue
  
**Prepare your dataset**
  
* Create a folder to contain all your dataset files
* Give this folder the name of your dataset, replacing spaces with underscores &rarr; `_`
* Move your dataset files (and ONLY your dataset files) into this folder

**Fork the colabfit-data repository**
  
* Click on the `Fork` dropdown menu near the upper right-hand side of the page
* Click on `Create new fork`
* Leave `Copy the main branch only` selected
* Click on `Create fork`
  
**Upload your dataset**
* Make sure you are on your fork of the repository
* Select `Add file` &rarr; `Upload files` from the right side of the activity bar
* Using your mouse, drag your **entire dataset folder** (containing all dataset files) onto the GitHub pane
  * Note: You must drag your files from your file explorer application onto the GitHub pane. The `choose your files` button will not allow you to upload a folder.
* Click on `Commit changes`. Leave `Commit directly to the main branch` selected.

**Submit a pull request**
* Click on `Compare & pull request`
    * You may need to find the `Contribute` button and click `Open pull request
* Select the `submit` branch as your PR base
    * The bar above the submission template should look something like:
    `base repository: colabfit/data-lake` `base: main` &larr; `head repository: your-GitHub/data-lake` `compare: main`
* Read through the pull request checklist and ensure you are prepared to submit
* Click `Create pull request`
  
## File expectations
  
### Content
Files should contain the data necessary to model atomic systems: atom types, atom coordinates, unit cell/lattice. They should also contain the values for calculated properties of the systems. For example properties, see [the current list of properties included in ColabFit](https://materials.colabfit.org/browse/property-definitions). We are most interested in files describing the relaxation trajectories of systems calculated at the quantum (e.g., CCSD) or DFT levels of theory.
  
### Format
Files in the .extxyz format (e.g., as implemented by ASE) are the most convenient to ingest, though we are able to work with other formats, including CIF, npy/npz and JSON.
  
Files may be compressed using a common compression format (tar, zip). Please do not use unusual or proprietary compression formats. If compressing a directory, keep in mind that GitHub has an upper limit on file sizes. It may be better to upload a larger number of smaller files.
  
