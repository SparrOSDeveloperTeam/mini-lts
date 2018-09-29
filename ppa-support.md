<center>| <a href="https://sparrosdeveloperteam.github.io/mini-lts">Home</a> | <a href="https://sparrosdeveloperteam.github.io/mini-lts/downloads">Downloads</a> | <a href="https://sparrosdeveloperteam.github.io/mini-lts/archives">Archives</a> | PPA Support |</center>

# PPA Support

Ubuntu Mini LTS releases support Ubuntu PPAs. Ubuntu Mini LTS acts similar to Ubuntu, allowing the person to add PPAs to their PC. To add a PPA to your system, you must run a series of commands:
```
sudo apt-add-repository ppa:user-name/ppa-name
sudo apt-get update
```
If however the above command does not work, the package `software-properties-common` may not be installed. To run it, you will need to use apt to install the package.

## Adding PPAs manually

Some people set up PPAs that require manual installation to set up the PPA. Using nano, edit the file `/etc/apt/sources.list` and add the PPA. When adding the PPA, you must add a line similar to this:
```
deb http://archive.ubuntu.com/ubuntu xenial main restricted universe multiverse
```
This line will install packages from all components at archive.ubuntu.com. Replace archive.ubuntu.com with the name of the page and xenial with your distribution release. In some instances, you may have to add a suite to the distribution such as `xenial-security` or `xenial-backports` depending on the suite.

For more information about PPAs, please visit [this page](https://github.com/SparrOSDeveloperTeam/mini-lts/wiki/ubuntu-ppa).
