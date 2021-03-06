[![Build Status](https://travis-ci.org/Sage-Bionetworks/synapseAnnotations.svg?branch=master)](https://travis-ci.org/Sage-Bionetworks/synapseAnnotations)

# Introduction

Sage Bionetworks derived standards for annotating content in Synapse.

# Schemas

Schemas are stored here in [Synapse Table Schema](http://docs.synapse.org/articles/tables.html) format. A schema is a list of [`Column Model`s](http://docs.synapse.org/rest/org/sagebionetworks/repo/model/table/ColumnModel.html) in JSON format.

Column types are required, and the valid types can be found [here](http://docs.synapse.org/rest/org/sagebionetworks/repo/model/table/ColumnType.html).

# Development

Internal development can be performed by branching from `master` to your own feature branch, making changes, pushing the branch to this repository, and opening a pull request. Pull requests against the master branch require a review before merging.

All pushed branches and pull requests are also tested through the continuous integration service [Travis CI](https://travis-ci.org/Sage-Bionetworks/synapseAnnotations). All JSON files are linted using [demjson's](deron.meranda.us/python/demjson/) `jsonlint` command line program.

When modifying the JSON schema files, we encourage you to install `demjson` to test your JSON files:

```
pip install demjson==2.2.4
```

or use the provided [requirements.txt](requirements.txt) file provided in this repository:

```
pip install -r requirements.txt
```
