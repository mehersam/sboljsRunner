# sboljsRunner

sboljsRunner is the test runner that tests the [sboljsRunner](https://github.com/SynBioDex/sboljs/releases) application for compliance of the [SBOL Standard](http://sbolstandard.org/). This test runner can be run as a standalone application, but it's intended purpose is to run it using the [SBOLTestRunner](https://github.com/mehersam/SBOLTestRunner). The application follows the Simple Round-trip approach as described within the github link to SBOLTestRunner. The application takes as input an SBOL data file and imports the file into pySBOLRunner and exports an SBOL data file. The purpose of this process is to ensure the sboljsRunner does not internally perform any data changes to SBOL data on import. Additionally, this process also identifies any unstated changes and test its overall compliance of the SBOL Standard.  

### Retrieving sboljsRunner

1. [Create](https://github.com/) a GitHub account.
2. [Setup](https://help.github.com/articles/set-up-git) Git on your machine.
3. Follow instructions on the [SBOLTestRunners](https://github.com/mehersam/SBOLTestRunners) Github repository to retrieve individual test runners.
4. [Download](https://nodejs.org/en/download/) NodeJS.
5. [Download](https://github.com/SynBioDex/sboljs/releases) sboljs.

### Using sboljsRunner

The sboljsRunner can be run through the command-line by using the following command: 

```
  node sboljsRunner.py <sbol_file_name> <retrieved_file_path> 
```

a. <sbol_file_name> is the SBOL data file to import. <br />
b. <retrieved_file_path> is the file path location where the exported file from SynBioHub will be placed. <br />
