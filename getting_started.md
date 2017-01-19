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

Run the following command from the `setup` directory to start a new instance (this will take a minute or so):

    $ bash setup_p2.sh

You should now see the instance within the AWS Console ([https://console.aws.amazon.com](https://console.aws.amazon.com)):

![aws_instance_running](documentation_images/running_instance.png)  

__Note: Make sure you stop the instance when not in use, as the cost is $0.90 per hour__

By running `setup_p2.sh` you will now have 2 new files in your setup directory, `fast-ai-commands.txt` and `fast-ai-remove.sh`. `fast-ai-commands.txt` contains a handy list of commands specifically for your instance. `fast-ai-remove.sh` is used to terminate your instance.



##Destroy the Instance (in case you need to)

    $ bash fast-ai-remove.sh

If this does not work, simply login to the AWS console, right click on the EC2 Instance, select: Instance State > Terminate.
