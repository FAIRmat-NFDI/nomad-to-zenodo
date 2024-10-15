# Publishing NOMAD Software from GitHub to Zenodo
This repository serves as a resource for NOMAD developers and the FAIRmat community, providing comprehensive instructions and guidelines for publishing software from GitHub to Zenodo. The guidelines will ensure that software is properly cited and archived, making it accessible and reusable according to FAIR principles.


## Introduction
The FAIRmat project produces several open source software products related to NOMAD. To ensure that these results are properly archived, cited, and FAIR compliant, the FAIRmat developers publish their software in the [FAIRmat Zenodo Community](https://zenodo.org/communities/fairmat_nfdi).

Zenodo integrates with GitHub to automatically archive software (repositories), and this process ensures that each version of the software receives a Digital Object Identifier (DOI) for proper citation.

## Prerequisites
- A Zenodo account (linked to your GitHub account)
- Permission to manage the GitHub repository you plan to publish.


## Steps to Publish on Zenodo
1. **Link GitHub to Zenodo**

Go to Zenodo and sign in. Then navigate to your account settings and link your GitHub account.
Once this is done, Zenodo will list all the public repositories from the FAIRmat organization as long as your account has permission to manage them. 
<div align="center">
<img src="images/link-github-to-Zenodo.gif" alt="Animated image (gif) showing the step of linking GitHub to Zenodo" width="800">
</div>


2. **Enable Zenodo Intergration**

In Zenodo, go to the "GitHub" section and find the repository you want to publish, then toggle the switch <img src="images/zenodo-switch.PNG" alt="Zenodo switch" width="30"> to turn on automatic preservation of your software.
By toggling the switch to **ON**, Zenodo will preserve the software for the long term, regardless of changes or possible deletion on GitHub. This will also allow Zenodo to automatically archive the repository, meaning that every time a new release is created, it will be captured and stored. A DOI is also generated, making the software citable. 

3. **Release a Version in GitHub**

To trigger the publication process, [create a new release in GitHub](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository). Make sure to add version tags (e.g., v1.0.0) and update release notes.This publication process and creating a DOI will proceed automatically after each new release. 
After the first release, a DOI badge that can be included in GitHub README will appear next to the repository on the Zenodo dashboard.
<div align="center">
<img src="images/enabled-repos-zenodo.PNG" alt="Zenodo switch" width="600"> 
</div>

## Best practice: Include a CITATION.cff file in your repository

To ensure that the published software contains all the metadata necessary for proper citation, a [CITATION.cff](https://citation-file-format.github.io/) file should be added to the root directory of the default branch in your repository. This file provides the necessary citation information, making it easier for others to properly cite your work.

### What is CITATION.cff file?
It is a plain text file with human- and machine-readable citation information for software. It is supported by GitHub, Zenodo, and Zotero. For more information click [here](https://citation-file-format.github.io/)

### How to create a citation.cff file to my repository?

- Please use the FAIRmat template available [here](template/).
- Copy the file and place it into the root directory of the default branch in your repository. Modify the placeholders (preceded by ##) with the relevant information specific to your project. Ensure all necessary fields are completed accurately for proper citation and metadata.

Some example files are also available [here](template/examples)
