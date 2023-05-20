# ClaroVoce

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
To pull and update:
```
git pull --recurse-submodules 
git submodule update --remote
```

