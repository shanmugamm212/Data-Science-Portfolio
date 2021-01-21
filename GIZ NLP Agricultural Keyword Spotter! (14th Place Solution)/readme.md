This repository contains solution for 17th place of GIZ NLP Agricultural Keyword Spotter competition
(https://zindi.africa/competitions/giz-nlp-agricultural-keyword-spotter/leaderboard)


### **Final solution overview:**
Final submission includes:
 - Augmentations : Gaussian noise, Pitch Shift, Short noise, Background noise, Speed augmenter, White noise, Pink noise,
                   Bandpass noise, Frequency masking
     - The sound files used for background and short noise downloaded from freesound.org
         - [street-scene-1 by saphe](http://freesound.org/people/saphe/sounds/150993/) 
         - [street-scene-3 by saphe](http://freesound.org/people/saphe/sounds/173955/)
         - [high-street-of-gandia-valencia-spain by jormarp](http://freesound.org/people/Jormarp/sounds/207208/)
         - [city-park-tel-aviv-israel by yonts](http://freesound.org/people/yonts/sounds/268903/)
     - Chunked original sound to 4 seconds in this [folder](https://github.com/shanmugamm212/Data-Science-Portfolio/tree/master/GIZ%20NLP%20Agricultural%20Keyword%20Spotter!%20(17th%20Place%20Solution)/bgn)
 - Models Used : Resnet18, Resnet34, Resnet50, Densenet121, Densenet169
 - Mean of all 5 models


### **Environments used**
 - OS - Ubuntu 18.04.5 LTS
 - Python - 3.7.4
 - CUDA - 11.1
 - Libraries from `requirements.txt`
 - Trained on one RTX 2060



### Reproduce steps:

 - copy all audio files without changing folder names from competition [portal](https://zindi.africa/competitions/giz-nlp-agricultural-keyword-spotter/data)
 - run `main.ipynb`
 
### **Credits**

 - Resampling input audio files (Pre-processing): https://gist.github.com/pmwaniki/fece16fff8f53ddb33d13df51054ab02
 - Augmentation Credits:
    * https://github.com/vlomme/Birdcall-Identification-competition
    * https://pypi.org/project/nlpaug/
    * https://github.com/iver56/audiomentations
 - FastAI for Datablock and Training the model : https://docs.fast.ai/


