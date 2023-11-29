# Contributing to a project maintained by the Davidson Group

First off, thanks for taking the time to contribute! 

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. Thank you!

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [Have a question or bug to report?](#have-a-question-or-bug-to-report)
- [Contributing to Code](#contributing-to-code)
- [Improving The Documentation](#improving-the-documentation)


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

#### Style
We expect that:
* Significant commenting/documentation of code is expected including:
   * A header to each file which describes it purpose, the authors/maintains and date of creation/modification.
   * Each function should have a comment to explain what it does and how.
   * Comments are expected within functions and inparicular for complex/convoluted lines of code.
* Adhere to common coding styles and practises for the language, including:
   * Do not use 'magic numbers', use a `#define` or otherwise explicitly given variable.
   * Modular design
   * Error checking. ie. checking that user input is in the expected format and print approporate error message if not.
* Use of other's code or algorithm (e.g. from stackoverflow, chatGPT or elsewhere):
   * Ensure that you have permission by checking the license.
   * Attribute code whenever possible, in a comment preferably, to acknowledge its ownership.
* Help/Usage information:
   * All software should make available help/useage information which print to the user.
   * Should also print the software name and version number
   * Should describe how to cite the software


#### Dependencies
We want our projects to be accessible and easy to compile, so have a preference for a minimal dependency count. If dependencies must be used, please ensure that they compile and are linked to stable versions. If possible, try to create
builds for major platforms such as x86 Linux and Mac.

#### Versioning
Our projects follow the following versioning system:

```
Flexiplex version 1 . 0 . 1
                  │   │   └ dev version, or 0 for release
                  │   └ minor version number
                  └ major version number
                   (reserved for large updates)  
```

### Improving The Documentation
Updates to the documentation are welcomed. The kinds of changes appropriate to the documentation are:
- Improved usage guidelines
- More examples showing common use cases
- Documentation of common exceptions which can occur

Updates can usually be made to the `gh-pages` branch of any given repository, since we use GitHub Pages for hosting.
