# DSE 200  
## Python setup  
* Pre-requisites
    * Python (so far, it looks like we only rely on version 2.X libraries)
    * Pip (download get-py.py and run `python get-py.py`)
    * Shell or any other
        * MacOS Recommended: iTerm2 or built-in
        * Windows Recommended: cygwin
        * Linux Recommended: bash/sh should be built-in!
### Installing Virtualenv and dependencies
#### Virtualenv
* This lets you install python packages in a subdirectory without affecting your base python installation
    * Great for isolating environments per-project
```
user@host:$ sudo pip install virtualenv // You'll want to have this installed on base/root python interpreter
user@host:$ cd ~                        // go to your home dir
user@host:$ virtualenv dse              // set up a virtual environment in a directory called 'dse'
user@host:$ source dse/bin/activate     // 'activate' the virtual environment for your current shell
(dse) user@host: $                      // the (dse) before your prompt means the virtual env is activated
```
#### Dependencies
* After you have virtualenv activated, download this requirements.txt file and run
```
pip install -r requirements.txt         // This tells pip to install all of the dependencies and the specified versions in the file
```