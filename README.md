# pyppbox-custpkg (Discontinued)

As [`pyppbox`](https://github.com/rathaumons/pyppbox) has reached mature state of its development, the latest `pyppbox` V3 now supports major operating systems like Windows/Linux/macOS, and it can be installed directly from `PyPI` or GitHub or be built from source. The same for some of its cutomized dependencies, [`pyppbox-torchreid`](https://github.com/rathaumons/torchreid-for-pyppbox) and [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox) are also available on `PyPI` and can be installed or built the same ways. For OpenCV with GPU support, `opencv-contrib-python` has been replaced with [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox), and the future prebuilt `.whl` will be released under its [GitHub releases](https://github.com/rathaumons/opencv-for-pyppbox/releases) directly. Therefore, this repo is now mark as discontinued. 

* Download new `pyppbox-opencv` v4.8.0 `.whl` from its [GitHub releases](https://github.com/rathaumons/opencv-for-pyppbox/releases)
* See how I build -> [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox)

---

The old prebuilt `.whl` files of our custom `opencv-contrib-python` with CUDA support are still available here:

* Download [**`.whl` for Python `3.10`**](py310)
* Download [**`.whl` for Python `3.9`**](py39)

Build info:

* Require `numpy>=1.24.2`
* Use the default path of CUDA & cuDNN `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\vxx.x`. 
  - -> Simply modify the `YOUR_PYTHON\Lib\site-packages\cv2\config.py` if the installation path of your CUDA is different
* The supported hardware for Python 3.9/3.10 + **CUDA 11.8/12.0**:
  ```
  NVIDIA GPU arch: 60 61 70 75 80 86 89
  NVIDIA PTX archs: 60 61 70 75 80 86 89
  ```
* The supported hardware for Python 3.9/3.10 + **CUDA 11.6/11.7**:
  ```
  NVIDIA GPU arch: 60 61 70 75 80 86
  NVIDIA PTX archs: 60 61 70 75 80 86
  ```
* OpenCV modules:
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
