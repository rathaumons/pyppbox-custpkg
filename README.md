# pyppbox-custpkg

* This repo hosts all pre-built WHLs of our customized packages for [`pyppbox`](https://github.com/rathaumons/pyppbox) such as `opencv_contrib_python` and `torchreid`.
* OpenCV modules of our `opencv_contrib_python`:
  ```
  OpenCV modules:
    To be built:                 aruco barcode bgsegm bioinspired calib3d ccalib core cudev datasets dnn dnn_objdetect dnn_superres dpm face features2d flann fuzzy gapi hfs highgui img_hash imgcodecs imgproc intensity_transform line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot python3 quality rapid reg rgbd saliency shape stereo stitching structured_light superres surface_matching text tracking video videoio videostab wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
    Disabled:                    cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping world
    Disabled by dependency:      -
    Unavailable:                 alphamat cvv freetype hdf java julia matlab ovis python2 sfm ts viz
    Applications:                -
    Documentation:               NO
    Non-free algorithms:         NO
  ```

## Note: 

* Our `opencv_contrib_python` uses the default path of CUDA & CUDNN `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.x`. 
* If your CUDA & CUDNN were installed in a different location, simply modify the `YOUR_PYTHON\Lib\site-packages\cv2\config.py` accordingly.
