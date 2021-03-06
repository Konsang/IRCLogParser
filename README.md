# IRCLogParser

[![Build Status](https://travis-ci.org/prasadtalasila/IRCLogParser.svg?branch=dev)](https://travis-ci.org/prasadtalasila/IRCLogParser) 
[![Code Climate](https://codeclimate.com/github/prasadtalasila/IRCLogParser/badges/gpa.svg)](https://codeclimate.com/github/prasadtalasila/IRCLogParser) 
[![Requirements Status](https://requires.io/github/prasadtalasila/IRCLogParser/requirements.svg?branch=dev)](https://requires.io/github/prasadtalasila/IRCLogParser/requirements/?branch=dev)    


The objective of this project is to utilize social network analysis techniques to examine the relationships between actors on the Internet Relay Chat(IRC) social networking service. The IRCLogParser is an application that accepts IRC log files from different channels and parses them to analyse the principles of interaction between IRC users. Study of these interactions on different levels helps us in deriving the local and global communication patterns between users on different channels. Therefore, IRCLogParser draws its inspiration from various fields such as data mining, graph theory and inferential modeling in order to form predictive models that help in understanding certain intricate characteristics of a social network. This involves analyzing graphs with IRC users(nodes) and their connections(edges), to study the details about various network graph properties such as density, size, node centrality, degree, connectedness etc.


<img src="https://github.com/prasadtalasila/IRCLogParser/blob/master/IRCLogParser/ext/sample_out/kubuntu-devel_4_10_2013_conversation.png?raw=true" width="400px"></img>
<img src="https://github.com/prasadtalasila/IRCLogParser/blob/master/IRCLogParser/ext/sample_out/infomap_CU.png?raw=true" width="400px"></img>


## Usage

The library's working has been modularised into many modules namely input, analysis, output, visualisation and validation. The [sample.py file](https://github.com/prasadtalasila/IRCLogParser/tree/master/sample.py) very comprehensively presents how one can use IRCLogParser for parsing and analysis.

Some of the visualisable sample outputs can be seen [here](https://github.com/prasadtalasila/IRCLogParser/tree/master/IRCLogParser/ext/sample_out/), giving an idea about IRCLogParser's capabilites.


## Documentation

IRCLogParser uses [Sphinx Python Documentation Genertor](http://www.sphinx-doc.org/en/stable/) for generating documentation of the library. The documentation is setup to work with [Google Style Docstrings](http://www.sphinx-doc.org/en/stable/ext/example_google.html) which eases the documentation writing process.

The documentation is deployed on the branch `gh-pages` who's updation has been made automatic by the a [bash script](https://github.com/prasadtalasila/IRCLogParser/tree/master/IRCLogParser/ext/docs_auto_deploy.sh) which otherwise requires to run `make html` in docs directory after every commit.

You can view the documentation hosted on `gh-pages` [here](http://prasadtalasila.github.io/IRCLogParser/).


## Testing

Presently, IRCLogParser has various end-to-end implemented which reside in the [test directory](https://github.com/prasadtalasila/IRCLogParser/tree/master/test/).
To run the tests locally on your machine, run `python -m unittest -v tests` in the test directory.


## Installation

IRCLogParser depends on various third-party libraries which are handled by [setup.py](https://github.com/prasadtalasila/IRCLogParser/tree/master/setup.py). 
Run `pip -v install -e .` in the root directory to install these dependencies.

## License

IRCLogParser is available under the [MIT License](https://github.com/prasadtalasila/IRCLogParser/tree/master/LISENCE.txt)

