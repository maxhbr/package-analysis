## Structure and Content of the Directory
The structure of the directory is quite straightforward. There will be one directory per analyzed package. The names of the directories are the same as the package names at the respective forge like Github or Sourceforge or any other.

Within the package directories there will be the following artifacts:
* Readme providing meta data of the package, like download location and if necessary comments and explanations about done curations
* SPDX tag value files, these files contain the identified and concluded licenses (the concluded licenses reflect the done curations if curations were done). There will be also comments about the curations in order to provide transparency why the specific curation was performed.
* Disclosure document, this documents aggregates all the concluded licenses, copyright notices and if necessary acknowledgments. These files are ready to use documents for being integrated in a so called "OSS disclosure document", which will be handed over to users of software incorporating the respective package. It is a simple text file.

## Naming Convention
In order to allow for automation and to ease the integration in build pipelines we follow a certain naming convention.

### Disclosure Documents 
The naming of the disclosure documents is: package name "-" package version "-OSS-disclosure.txt". In case you have analyzed gnutls 3.7.8 the corresponding name of the disclosure document is: gnutls-3.7.8-OSS-disclosure.txt

### SPDX files 
The naming of the spdx tag value files is: package name "-" package version "-SPDX2TV.spdx". In case you have analyzed gnutls 3.7.8 the corresponding name of the spdx file is: gnutls-3.7.8-SPDX2TV.spdx

## Improving the Artifacts
Since all files are text files, they can easily be reviewed. In case you detect an error or have doubts please file an issue against the specific file.

## Improving Trust in the Accuracy of the provided Data
In case you have reviewed and everything is correct in your opinion it would be very nice if you add your name to the list of reviewers listed in the Readme file.