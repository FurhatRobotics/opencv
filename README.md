# OpenCV: Open Source Computer Vision Library

## Videoio Module

### APIs Introduced

* bool getDevices(int &devices);
* bool getDeviceInfo(int device, String &deviceName, String &vid, String &pid, String &devicePath);
* bool getFormats(int &formats);
* bool getFormatType(int format, String &formatType, int &width, int &height, int &fps);
* bool setFormatType(int format)
* bool get(int propId, long &min, long &max, long &steppingDelta, long &supportedMode, long &currentValue, long &currentMode, long &defaultValue);
* bool set(int propId, long value, long mode);

### APIs Explanation

#### bool getDevices(int &devices);

* Get total number of camera devices connected to the port.


#### bool getDeviceInfo(int device, String &deviceName, String &vid, String &pid, String &devicePath);

* Get specific camera device information such Device name, Device path, VendorID and productID.


#### bool getFormats(int &formats);

* Get total number of video formats supported by the camera device.


#### bool getFormatType(int format, String &formatType, int &width, int &height, int &fps);

* Get video resolution, video format and fps supported by the camera


#### bool setFormatType(int format);

* Set the video format, resolution and fps to the device. 


#### bool get(int propId, long &min, long &max, long &steppingDelta, long &supportedMode, long &currentValue, long &currentMode, long &defaultValue);

* Get specific UVC Property(Brightness, Contrast,...) minimum value, maximum value, current value, default value, steppingDelta, current mode and supported mode.


#### bool set(int propId, long value, long mode);

* Set specific UVC Property(Brightness, Contrast, Hue,...) value and mode.



## OpenCVCam Command Line Application

* OpenCVCam command line application can be used to access the UVC settings, HID settings, Streaming and Image capture of any e-con System cameras in both Windows and Linux.



## How to Use

* OpenCV can be downloaded from [here](https://github.com/opencv/opencv)
```
* cd opencv
```

```
* git checkout 3.3.1
```

* Replace Videoio module from OpenCV with [this videoio module](https://github.com/econsystems/opencv/tree/master/Sources)
* Build OpenCV using [this Installation manual](https://github.com/econsystems/opencv/tree/master/Documents)
* Information on how to use those newly Introduced APIs were [explained in API Documentation](https://github.com/econsystems/opencv/tree/master/Documents)
* OpenCVCam command line application can be downloaded [from here](https://github.com/econsystems/opencv/tree/master/Sources), which is used to access OpenCV APIs
* Run Sample application using [this user manual](https://github.com/econsystems/opencv/tree/master/Documents)
