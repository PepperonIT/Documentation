If you cannot install pip2 in ubuntu run `wget https://bootstrap.pypa.io/pip/2.7/get-pip.py`
and then `sudo python2 get-pip.py`

Pepper controller can be found at `https://github.com/incognite-lab/Pepper-Controller`
and can be cloned with
`git clone https://github.com/incognite-lab/Pepper-Controller.git`

On linux you have to install python-tk and then run the installation `apt install python-tk`

To install packages run `pip2 install -r ./requirements.txt` or
`python2 -m pip install -r ./requirements.txt`

To install required packages which isn't included in requirements run
`pip2 install opencv-python==4.2.0.32`