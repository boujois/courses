#Getting Started

##AWS CLI

Install Amazon AWS CLI tool. See full instructions [here](http://docs.aws.amazon.com/cli/latest/userguide/installing.html).

__Linux or OSX:__

    $ sudo pip install awscli

__Windows:__

    > pip install awscli

Verify your installation by running:

    $ aws --version

You should see something like:

    aws-cli/1.11.30 Python/2.7.10 Darwin/16.3.0 botocore/1.4.87

Configure AWS CLI with your Access Key, Secret Access Key & Region preference:

    $ aws configure

##Anaconda (Python)

Download Anaconda from [here](https://www.continuum.io/downloads). Make sure you pick the Python 2.7 Installer.

##Cygwin (Windows only)

If you are using Windows, you will need a Bash shell. The easiest solution is to install Cygwin from [here](https://cygwin.com/install.html). Make sure when you install that you ensure the `wget` package is included:

![cygwin_wget](documentation_images/Cygwin-6-Select-wget.png)

##Fast.ai Scripts

Navigate to the `setup` directory:

    $ cd setup

Add the aliases:

    $ source aws-alias.sh

##Create an Instance

    $ bash setup_p2.sh

##Destroy the Instance (in case you need to)

    $ bash fast-ai-remove.sh
