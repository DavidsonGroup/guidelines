# Contributing to a project maintained by the Davidson Group

First off, thanks for taking the time to contribute! 

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. Thank you!

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [Have a question or bug to report?](#have-a-question-or-bug-to-report)
- [Contributing to Code](#contributing-to-code)
- [Documentation](#documentation)


## Code of Conduct

This project and everyone participating in it is governed by the
[Davidson Group Code of Conduct](https://github.com/DavidsonGroup/guidelines/blob/main/CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code.

### Have a question or bug to report?

Before you ask a question, check the relevant tool's documentation, existing "Dicussion" board, as well as github Issue to see if your questions has already been answered. 

If it hasn't we recommend posting general questions to the github repository's Discussion e.g. [Flexiplex Discussion]([https://github.com/DavidsonGroup/flexiplex/issues/new](https://github.com/DavidsonGroup/flexiplex/discussions)).

For bugs, please post add an item to github repository's Issues e.g. [Flexiplex issue](https://github.com/DavidsonGroup/flexiplex/issues). To help us identify the problem as quickly as possible, please provide the following information:
- Which version you installed and how you installed it (including your gcc version if applicable)
- The exact command you ran including an options and a description of the input data you provided.
- Whether the software would run another other scenarios (different version, different set of options, or different input data). Where we provide test datasets, please run these first before submitting a bug and report the result of the test run.
- The error message and any other output from the program
- The system you ran on: OS, Platform and Version (Linux, macOS, x86, ARM), available memory, threads etc.
- If you can provide us with toy dataset to reproduce the issue, this will be a great help! 


### Contributing to Code
#### Testing
Please ensure that your contributions build and pass all testing prior to submitting a pull request. 

Packages maintainers are responsible for contructing a set of test cases which must be run on each pull request. The tests may be small, but must cover all common usages of the tool. Ideally these will be added to a Github Action for continuous integration.

#### Coding Style
We expect that:
* Significant commenting/documentation of code is expected including:
   * A header to each file which describes it purpose, the authors/maintains and date of creation/modification.
   * Each function should have a comment to explain what it does and how.
   * Comments are expected within functions and inparicular for complex/convoluted lines of code.
* Adhere to common coding styles and practises for the language, including:
   * Do not use 'magic numbers', use a `#define` or otherwise explicitly given variable.
   * Modular design.
   * Variable names are descriptive.
   * Error checking. ie. checking that user input is in the expected format and print approporate error message if not.
* Use of other's code or algorithm (e.g. from stackoverflow, chatGPT or elsewhere):
   * Ensure that you have permission by checking the license.
   * Attribute code whenever possible, in a comment preferably, to acknowledge its ownership.
* Help/Usage information:
   * All software should make available help/useage information which print to the user.
   * Should also print the software name and version number
   * Should describe how to cite the software
* Installation:
     * A means to easily install/compile the package including dependencies should be provided. For example with Makefiles and Config. files.
     * The package should have minimal dependencies to help in installation and maintainence. If dependencies are used, please ensure that they compile and are linked to stable versions.
     * If possible, try to create builds for major platforms such as x86 Linux and Mac, and submit the package to package managers like bioconductor, bioconda or brew.


#### Versioning
Our projects follow the following versioning system:

```
Flexiplex version 1 . 00 . 1
                  │   │   └ dev version, or absent for a release
                  │   └ minor version number
                  └ major version number
                    
```
The major version number should be incremented for large updates such as signficant restructing of the code that results in computational efficiency changes, new major features, or any changes that break backwards compatibilty (e.g. error when old command line options are provided by the user).

The minor version number should be incremented for all other releases.

The version number is to be updated in the relevant sections of the code and a tagged added through Github (non-dev version only).

For example, Flexiplex 1.00.1 is a developemental version. Once a stable release is ready (timing at the discretion of the software owner), the version should be incremented to version 1.01 in the code, tagged on Github and a release created on Github which describes the changes. A tarball asset may also be uploaded for the package (this is somewhat redundant, but allows download numbers to be tracked). Immediately following the release, the version should be incremented to the next dev version (1.01.1). 

### Documentation

All sofware packages should have associated user documentation, such as GitHub Pages. The documentation should describe:
* What the software is
* How the software works
* How it can be installed
* How is can be run
* What the software outputs in detail
* How to get help and report issues
* A short tutorial based on a small example dataset, with link to the data
* Links to relevant documents such as papers which derscribe the software
* How the software should be cited

Updates to the documentation are welcomed, and may include:
- Improved usage guidelines
- More examples showing common use cases
- Documentation of common exceptions which can occur

