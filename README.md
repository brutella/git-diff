git-diff
========

Compare git branches, tags and commits in your favourite diff tool.

## Installation

Copy `git-diff` in some folder under `$PATH`, e.g. `/usr/local/bin/`.

## Usage

Run 

    git-diff master develop

from a git repo's root folder to see the diff from branch `master` to `develop` which may look someting like this.

![opendiff Example](./opendiff-example.png?raw=true)

From there on your can visually compare the diff.

![diff Example](./opendiff-example-diff.png?raw=true)

You can compare between branches, tags or commits.

    # tags
    git-diff 1.0.0 1.0.1
    
    # commits
    git-diff 1be7447 3e52081
    
    # compare master to tag
    git-diff 1.0.0 master
    

The scripts uses git's preferred diff tool specified for the config `diff.tool` or `opendiff` if no git diff tool is configured.

## Contact

Matthias Hochgatterer

Github: [https://github.com/brutella/](https://github.com/brutella/)
Twitter: [https://twitter.com/brutella](https://twitter.com/brutella)

## License

git-diff is availabe under ISC license. See the LICENSE file for more info.
