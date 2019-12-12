# git-clone-repo
Utility script for cloning a git repository to a temporary folder

## Download/Install

    curl -sSL 'https://raw.githubusercontent.com/pcoltau/git-clone-repo-to-temp-dir/master/git-clone-repo.sh' -o git-clone-repo.sh
    
	chmod +x git-clone-repo.sh

    ./git-clone-repo.sh <git-repo>

## Usage

    >./git-clone-repo.sh -h
    
    git-clone-repo.sh [-h] [-v] [--branch <branch>] [--tag <tag>] <git-repo>

	This script will checkout a git repository to a temporary directory and return the path to the directory

	Example:
	  git-clone-repo.sh "Safetrack/trackunit-go-ios"

	  - will checkout the master branch of the "trackunit-go-ios" repository

	Options:
	      --branch         Define the branch to checkout. Default is 'master'. Cannot be combined with "--tag".
	      --tag            Define the tag to checkout. Cannot be combined with "--branch".
	  -h, --help           Display this help and exit
	      --version        Output version information and exit