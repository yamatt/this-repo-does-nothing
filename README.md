# This Repo Does Nothing
I'm growing concerned about the recent trend in adding configuration and meta data to repository root directories. These are files that by themselves do absolutely nothing but are necessary for other things using the repository to work.

I can see us (as a community) getting to the point where our repository roots are stuffed with files that do nothing but describe the repo.

## Complaints
* They tend to be hidden files, but that just hides the mess, sweeps it under the carpet.
* They have no reason to be in the root, they could easily be in another directory.

## Solution
Lets just agree to put all these files in a standardised directory, lets called it `.config`. A simple, single source for all these files to be. You can even set up the programs that look for these files to try the root and this directory.

## How you can help
Submit pull requests to this repo that contain configuration files that could easily be stored in another directory.

## Exceptions
There are some reasonable exceptions, these are files that humans tend to interact with often. For example:
* `setup.py`
    Python configuration file used to install, test and perform common actions.
* `package.json`
    A configuration and meta data file that is used to install, test and perform other common actions.
* `configure`
    A file that sets up an environment for install.
* `Makefile`
    Used for running commands on a directory.

Arguably these could also all be placed in the `.config` directory, however there would be a lot of stuff would break without them.
