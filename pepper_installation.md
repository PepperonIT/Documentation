
# Python 2.7
## Windows
Install python 2.7 on [python installers](https://www.python.org/downloads/release/python-2718/).

## Linux
### Ubuntu/Debian
On ubuntu it is not enough to have ubuntu, you also need to install python2.7-dev: \
To install python 2.7 run the command:
```
sudo apt install python2.7 
```

Then to install python2.7-dev run:
```
sudo apt install python2.7-dev
```

### Arch Linux / Manjaro
On arch-based systems it is necessary to build python 2 from source. The source release can be downloaded from the official python website [found here](https://www.python.org/downloads/release/python-2718/)(2.7.18).

For installing the Gzipped source tarball version you can do the following:

First you unzip the downloaded archive:
```
tar -xzvf Python-2.7.18.tgz
```

After that, you navigate to the unzipped folder. For more detailed installation instructions, it is suggested to read the README. The short simple version follows:

First we run the configuration file:
```
./configure
```

When that has finished you run:
```
make
```

This creates an executable in /usr/local/. Next do:
```
su root
```

Then install python with:
```
make install
```

After it has finished, python 2 should be successfully installed
# naoqi
## Ubuntu
Download and extract the [Python SDK](https://developer.softbankrobotics.com/pepper-naoqi-25-downloads-linux).

The SDK then needs to be added to the python path, to get the path open the naoqi folder in a terminal and navigate to:
> ~/lib/python2.7/site-packages/

In the terminal run the "path working directory" command:
```
pwd
```
This prints out the path we need to add to python. To do this open the bashrc file and append the export statement, this can for example be:
```
export PYTHONPATH=${PYTHONPATH}:/home/anders/Documents/naoqi/pynaoqi-python2.7-2.5.7.1-linux64/lib/python2.7/site-packages
```

To verify that it works, open a new terminal and run:
```
python2.7
```
And import naoqi
```
import naoqi
```

To further verify, you can run:
```
from naoqi import ALProxy
```
```
tts = ALProxy("ALTextToSpeech", "130.240.238.32", 9559)
```
```
tts.say("Hello, world!")
```
