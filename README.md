# GetTheZodi
In the night sky, we're used to seeing stars. That is, if we're not seeing clouds.
If you're lucky, you can see traces of the Milky Way.

That's with visible light, what our human eyes can see. But there's so much interesting stuff happening at infrared wavelengths!

The problem is that, in the infrared, the Milky Way starts getting mixed up with more "local" light, that from within our solar system.

This repository is a quick in dirty experiment, born purely out of curiosity (read: boredom and perhaps frustration with me "real" PhD research.) I just wanted to see if a simple component separation approach could get us anywhere near a clean separation of light from the Milky Way and that of the solar system's dust (called "Zodiacal dust" by those who actually study it-- just ask Dr. Brian May, of Queen!), without assuming a physical model for either one.

In a nutshell: I threw the COBE-DIRBE near to far infrared all-sky maps at principal component analysis (PCA), indpeendent component analysis (ICA), and non-negative matrix factorization (NMF) algorithms. These examples are based on `scikit-learn`'s implementations of those algorithms, but it might be a fun excercise to write them yourself in `numpy` (actually, pretty trivial at least when it comes to PCA). 

The reason I use the COBE-DIRBE data hear, quite honestly, is because it's low-resolution and thus quite easy to make a demonstration out of. All of the wavelengths, from the Milky Way-dust dominated, to the stellar light dominated emission are covered in a consistent and conveniently available data format.

We could also experiment by combining other space satellite data with DIRBE, or look exclusively at the higher resolution data from Planck, AKARI and IRAS.




Give it a try on Binder!

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/aaroncnb/GetTheZodi/master?filepath=BlindZodiSeparation_ExampleDIRBE.ipynb)
