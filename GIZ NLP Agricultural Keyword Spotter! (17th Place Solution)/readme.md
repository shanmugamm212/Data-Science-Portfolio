This repo contains solution for 17th place of GIZ NLP Agricultural Keyword Spotter competiton
(https://zindi.africa/competitions/giz-nlp-agricultural-keyword-spotter/leaderboard)


### **Final solution overview:**
Final submission includes:
 - Augmentations : Gaussion noise, Pitch Shift, Short noise, Background Noise, Speed Augmenter, white noise, Pink noise,
                   bandpass noise, Frequency Masking
     * The sound files used for background and short noise downloaded from freesound.org
            * [street-scene-1 by saphe](http://freesound.org/people/saphe/sounds/150993/) 
            * [street-scene-3 by saphe](http://freesound.org/people/saphe/sounds/173955/)
            * [high-street-of-gandia-valencia-spain by jormarp](http://freesound.org/people/Jormarp/sounds/207208/)
            * [city-park-tel-aviv-israel by yonts](http://freesound.org/people/yonts/sounds/268903/)
     * Cropped original sound to 4seconds in this [folder]()
 - Models Used : Resnet18, Resnet34, Resnet50, Densenet121, Densenet169
 - Mean of all 5 models


### **Environments used**
 - OS - Ubuntu 18.04.5 LTS
 - Python - 3.7.4
 - CUDA - 11.1
 - libraries from requirements.txt
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


