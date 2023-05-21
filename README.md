# ClaroVoce

## Prerequisites
CMake version 3.16 or higher
Python


## Submodules
This repo uses submodules coqui-ai/TTS.git
While cloning use the --recurse-submodules flag
```
git clone --recurse-submodules https://github.com/mainak33/ClaroVoce.git
```
To manually add the submodule in the parent directory (if cloned without the --recurse-submodules):
```
git submodule add ../../coqui-ai/TTS.git extern/TTS
```

The TTS repo uses the branch main and not the default origin. Use any of the following command to set the default branch for the submodule:
```
git submodule set-branch --branch main extern/TTS
git config -f .gitmodules submodule.extern/TTS.branch main
```

To pull and update:
```
git pull --recurse-submodules 
git submodule update --remote
```

#Python venv and install
It is recommended to install TTS inside a venv
```
python -m venv <path to venv>
cd <path to venv>
pip install TTS
pip install -e <path to repo>/extern/TTS
```
To activate the venv on bash:
```
source <path to venv>/bin/activate
```
To create an example wav file in the venv:
```
python3 <path to repo>testTTS.py
```
