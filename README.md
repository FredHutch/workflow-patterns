# Common Workflow Patterns

[GO TO THE WIKI](https://github.com/FredHutch/workflow-patterns/wiki)

[SUBMIT AN ISSUE](https://github.com/FredHutch/workflow-patterns/issues)

## Mission Statement

Repository to keep track of commonly used elements of computational workflows, e.g. Nextflow and Cromwell.

With the increasing popularity of workflow managers for data intensive analysis pipelines (such as
with 'omics technologies like high-throughput genome sequencing instruments), workflow developers
may find themselves reusing individual steps across multiple projects. This repository is intended
to be a place for workflow developers to contribute and source snippets of code which can be used
to build workflows.

While this repository is not intended to be specific to any single workflow language, it has been
largely enabled by the features added to Nextflow in Version 20 (DSL-2) in which individual processes
can be imported as modules which are then composed into workflows. Using this repository, we hope to
enable workflows developers to use the code hosted here to build a set of modules which are easily
and quickly combined into a useful workflow.

## Structure

In this first attempt, we will use two aspects of GitHub in order to organize this repository. The
wiki will be used to organize the code snippets, while the issues will be used to discuss changes
and contributions to the wiki. The wiki can only be modified by a set of approved contributors, and
so newcomers can propose to add a new module (or report an issue with an existing module) by creating
an issue.

## How to Contribute

### New Modules

If you have a new module that you would like to add, submit an issue which includes:

- Description of inputs
- Description of outputs
- Description of parameters
- Description of container with link to source Dockerfile
- Description of how the module should be used
- Suggestion for the category that this module may fall into
- Workflow language used
- Code for module
- How you would like to be cited

Once the issue has been reviewed by another user, one of the approved contributors will add it
to the wiki in the indicated category.

**NOTE:** There are many ways to write modules which do largely the same thing. 
Do not hesitate to contribute additional modules which accomplish the same task in a different way!
The wiki will be set up to include multiple modules which accomplish the same task, citing each
contributor individually.

### Reporting Bugs

If you have used a module and found that it does not behave as expected, file a bug report
which includes:

- The module code which resulted in the error
- A link to the location of the module in the wiki
- The error message
- A suggestion for what modification should be made (changing code, removing the module, etc.)

**NOTE:** The maintainers of this repository are not expected to debug modules, so any serious
errors with no obvious fix may just be reported as a warning in the wiki. If the original author
can find no fix, then the module may just be removed from the wiki.
