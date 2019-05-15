This file contains three parts: 

1) test data including one simulated data(Fig. 3)  and one experimental real data (Fig. 1)
2) the executable .pyc files
3) the visualization look-up tables 'error map.lut'

Prerequisites:
1. OpenCv-python
2. matplotlib v3.0.3
3. scipy v1.2.1
4. scikit-image v0.15.0
5. Pillow v6.0.0
5. Fiji software (https://imagej.net/Fiji/Downloads)


To test our algorithm, pelease print command 
'python sr-ssim_main.pyc highbg' for high-level background simualted data 
or 'python sr-ssim_main.pyc actin' for experimental actin data.

The outputs are under the path '../data/actin/storm/output' for actin data and '../data/highbg/storm/output' for high-level background data. The ouputs includes .tif errormap and score.txt with SR-SSIM index value.

To visualize the errormap first please put the error map.lut under the luts file of Fiji then open the errormap with Fiji you can use Fiji->Image->Lookup Tables->error map to see the artifacts distribution heat map.

To simplify the part preprocess step which finished by ImageJ and some java code, we directly provide all the inputs that the algorithm needs including the resized widefield image, the degraded super-resolution image and the mask. If you need other materials, please contact  corresponding author Prof. Fa Zhang (zhangfa@ict.ac.cn).



