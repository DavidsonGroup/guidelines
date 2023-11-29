# Contributing to a project maintained by the Davidson Group

First off, thanks for taking the time to contribute! 

All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. Thank you!

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [I Have a Question](#i-have-a-question)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
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
Please ensure that your contributions build and pass all testing prior to submitting a pull request. If your change involves the implementation of new features, please provide
tests (in unit test for or otherwise) which make an attempt to cover all edge cases.

#### Style
We expect that:
* All code and changes are well documented
* Functions should have a comment to explain what they do, no matter if it's an internal or user-facing function.
* Complex/convoluted lines of code should have their function documented
* Do not use 'magic numbers', use a `#define` or otherwise explicitly given variable. Even better allow it to be changed with a command-line flag, configuration file, environment variable, or `.env` file.
* If using code from the internet, ensure that you have permission by checking the license. Attribute code whenever possible, in a comment preferably, to acknowledge its ownership.
* If you find yourself using the same code twice or more, consider putting it into a well-documented function.
* You try to follow existing code style whenever possible

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
