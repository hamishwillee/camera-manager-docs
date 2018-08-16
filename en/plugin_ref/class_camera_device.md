# CameraDevice Class Reference
`#include: CameraDevice.h`

----


The [CameraDevice](class_camera_device.md) class is base for different camera devices. 


## Data Structures


struct [Size](struct_camera_device_1_1_size.md)

## Public Types


Type | Description
--- | ---
enum [Status](#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | 
enum [State](#class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61) | 

## Public Member Functions


Type | Name | Description
---: | --- | ---
&nbsp; | [CameraDevice](#class_camera_device_1af098dec1e516dff464b6c80389ab043f) () |
&nbsp; | [~CameraDevice](#class_camera_device_1ac885198479887e5a3779a818e07e9917) () |
std::string | [getDeviceId](#class_camera_device_1a70db218e718da6012de003d593fa2618) () const =0 |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getInfo](#class_camera_device_1aefb7f3cf8a535c8ff3fa1cf3c162ae4d) ([CameraInfo](struct_camera_info.md) & camInfo)const =0 |
bool | [isGstV4l2Src](#class_camera_device_1a37b08fca3defd1f7451424f9ae5cb0e8) () const =0 |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [init](#class_camera_device_1af4cf16a4efdb539f7f893230510780ca) (CameraParameters & camParam)=0 |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [uninit](#class_camera_device_1ac37298ea498429dabf8190247c89217d) ()=0 |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [start](#class_camera_device_1a43d7d489571cb7e13b026dc140c89579) () |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [start](#class_camera_device_1ae268c53a698f99541c9eff0a7c527037) (const std::function< void([CameraData](struct_camera_data.md) &)> cb) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [stop](#class_camera_device_1a4751d38e9d16860e1f6b4a43bace0700) () |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [read](#class_camera_device_1a25677bf37eac5b14352d097336838e57) ([CameraData](struct_camera_data.md) & data) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setParam](#class_camera_device_1a0af085aad921e78746fd843c3226d8d6) (CameraParameters & camParam, const std::string param, const char * param_value, const size_t value_size, const int param_type) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [resetParams](#class_camera_device_1a8e1da0f7e9a50cc94daa48c6ad9f35b7) (CameraParameters & camParam) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setSize](#class_camera_device_1a2d9c276ac6bd3efa6f6aab14dfe4f379) (const uint32_t width, const uint32_t height) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getSize](#class_camera_device_1ae510762e28618ee6b51d3faa0f500de2) (uint32_t & width, uint32_t & height)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getSupportedSizes](#class_camera_device_1a0905c35d684dc07bad503d28c00a7941) (std::vector< [Size](struct_camera_device_1_1_size.md) > & sizes)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setPixelFormat](#class_camera_device_1a69ea0555f03cc76064efcb466d573ee1) (const CameraParameters::PixelFormat format) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getPixelFormat](#class_camera_device_1a7eb98b7258304d850cd5b2f6299728c3) (CameraParameters::PixelFormat & format)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getSupportedPixelFormats](#class_camera_device_1a7b01831ca40b07d047abb8e26c2080f7) (std::vector< CameraParameters::PixelFormat > & formats)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setMode](#class_camera_device_1a4aeb312e3ea2e9b97a5f9934255d498a) (const CameraParameters::Mode mode) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getMode](#class_camera_device_1a3c375f481b80d8c73f34824c46cb60da) (CameraParameters::Mode & mode)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getSupportedModes](#class_camera_device_1ae0b18c9f04acf1e3a9e02c7f964335c9) (std::vector< CameraParameters::Mode > & modes)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setFrameRate](#class_camera_device_1a969307ab2e83139176e762199f86b97b) (const uint32_t fps) |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getFrameRate](#class_camera_device_1a9802d319f82f5b902be109e29253bc9d) (uint32_t & fps)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [getSupportedFrameRates](#class_camera_device_1a132e700f2e5fd086e62039da38536cf5) (uint32_t & minFps, uint32_t & maxFps)const |
[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) | [setCameraDefinitionUri](#class_camera_device_1a7e4bca0adbc992262e3e5a14ae7df2eb) (const std::string uri) |
std::string | [getCameraDefinitionUri](#class_camera_device_1a4d3516539d39ec80f52884acbc3b54a6) () const |
std::string | [getOverlayText](#class_camera_device_1a20c1581a6a31fd5c9a71728f39e0be3d) () const |


## Constructor & Destructor Documentation


### CameraDevice() {#class_camera_device_1af098dec1e516dff464b6c80389ab043f}
```cpp
CameraDevice::CameraDevice()
```


### ~CameraDevice() {#class_camera_device_1ac885198479887e5a3779a818e07e9917}
```cpp
virtual CameraDevice::~CameraDevice()
```


## Member Enumeration Documentation


### enum Status {#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4}


Possible return values from class methods.

Value | Description
--- | ---
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4ad0749aaba8b833466dfcbb0428e4f89c"></span> `SUCCESS` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4a0a306e577f7923ac78d86a60bee66966"></span> `ERROR_UNKNOWN` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4af295a0c3e37c94f078e1c5476479132d"></span> `INVALID_ARGUMENT` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4a5e6a8de74c8f7d4b04d91a3dc3bf7659"></span> `INVALID_STATE` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4afe39af6ff8b4f14f5759e4d70bba6ebc"></span> `NO_MEMORY` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4a49c22d7d0c1b740088957db49b4fc4b0"></span> `PERM_DENIED` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4adbe2cbac46ffa8283747010d8e1e6396"></span> `TIMED_OUT` |  
<span id="class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4a5343bcd21aad65124478a61831f6949e"></span> `NOT_SUPPORTED` |  

### enum State {#class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61}


Possible states of the object.

Value | Description
--- | ---
<span id="class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61a458ab6c6280de70d59093cdb5887b2ee"></span> `STATE_ERROR` |  
<span id="class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61a667adf1721ecf31975b473ea51005d04"></span> `STATE_IDLE` |  
<span id="class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61abb47b9b1d888741b1d94f3f060281299"></span> `STATE_INIT` |  
<span id="class_camera_device_1af1243dea719e4bc73cbc97222e9e5b61a8fed89d3af776e8151350645afaece9d"></span> `STATE_RUN` |  

## Member Function Documentation


### getDeviceId() {#class_camera_device_1a70db218e718da6012de003d593fa2618}
```cpp
virtual std::string CameraDevice::getDeviceId() const =0
```


Get the identifier of the Camera Device.

**Returns**

&emsp;std::string - string Camera device Id.

### getInfo() {#class_camera_device_1aefb7f3cf8a535c8ff3fa1cf3c162ae4d}
```cpp
virtual Status CameraDevice::getInfo(CameraInfo &camInfo) const =0
```


Get camera device information.

**Parameters**

* [CameraInfo](struct_camera_info.md)& **camInfo** - Camera Information

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### isGstV4l2Src() {#class_camera_device_1a37b08fca3defd1f7451424f9ae5cb0e8}
```cpp
virtual bool CameraDevice::isGstV4l2Src() const =0
```


Check if gstreamer v4l2src element can be used to capture from the Camera Device.

**Returns**

&emsp;bool - bool True if gstreamer v4l2src element supported, otherwise false

### init() {#class_camera_device_1af4cf16a4efdb539f7f893230510780ca}
```cpp
virtual Status CameraDevice::init(CameraParameters &camParam)=0
```


Initialize camera device.

**Parameters**

* CameraParameters& **camParam** - Camera Parameters with default values filled

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### uninit() {#class_camera_device_1ac37298ea498429dabf8190247c89217d}
```cpp
virtual Status CameraDevice::uninit()=0
```


Uninitialize camera device.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### start() {#class_camera_device_1a43d7d489571cb7e13b026dc140c89579}
```cpp
virtual Status CameraDevice::start()
```


Start camera device.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### start() {#class_camera_device_1ae268c53a698f99541c9eff0a7c527037}
```cpp
virtual Status CameraDevice::start(const std::function< void(CameraData &)> cb)
```


Start camera device in asynchronous mode.

**Parameters**

* const std::function< void([CameraData](struct_camera_data.md) &)> **cb** - Callback function to receive camera data

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### stop() {#class_camera_device_1a4751d38e9d16860e1f6b4a43bace0700}
```cpp
virtual Status CameraDevice::stop()
```


Stop camera device.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### read() {#class_camera_device_1a25677bf37eac5b14352d097336838e57}
```cpp
virtual Status CameraDevice::read(CameraData &data)
```


Read camera images from camera device.

**Parameters**

* [CameraData](struct_camera_data.md)& **data** - [CameraData](struct_camera_data.md) to hold image and meta-data.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setParam() {#class_camera_device_1a0af085aad921e78746fd843c3226d8d6}
```cpp
virtual Status CameraDevice::setParam(CameraParameters &camParam, const std::string param, const char *param_value, const size_t value_size, const int param_type)
```


Set parameter of the camera device.

**Parameters**

* CameraParameters& **camParam** - Camera Parameters.
* const std::string **param** - Name of the parameter.
* const char\* **param_value** - Value of the parameter to be set.
* const size_t **value_size** - Length of the value of the parameter.
* const int **param_type** - Type of the parameter.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### resetParams() {#class_camera_device_1a8e1da0f7e9a50cc94daa48c6ad9f35b7}
```cpp
virtual Status CameraDevice::resetParams(CameraParameters &camParam)
```


Reset parameters of the camera device to default.

**Parameters**

* CameraParameters& **camParam** - Camera Parameters.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setSize() {#class_camera_device_1a2d9c276ac6bd3efa6f6aab14dfe4f379}
```cpp
virtual Status CameraDevice::setSize(const uint32_t width, const uint32_t height)
```


Set camera image resolution.

**Parameters**

* const uint32_t **width** - Width of the output image to be set.
* const uint32_t **height** - Height of the output image to be set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getSize() {#class_camera_device_1ae510762e28618ee6b51d3faa0f500de2}
```cpp
virtual Status CameraDevice::getSize(uint32_t &width, uint32_t &height) const
```


Get camera image resolution.

**Parameters**

* uint32_t& **width** - Width of the output image set.
* uint32_t& **height** - Height of the output image set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getSupportedSizes() {#class_camera_device_1a0905c35d684dc07bad503d28c00a7941}
```cpp
virtual Status CameraDevice::getSupportedSizes(std::vector< Size > &sizes) const
```


Get list of supported camera image resolution.

**Parameters**

* std::vector< [Size](struct_camera_device_1_1_size.md) >& **sizes** - Vector of sizes supported.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setPixelFormat() {#class_camera_device_1a69ea0555f03cc76064efcb466d573ee1}
```cpp
virtual Status CameraDevice::setPixelFormat(const CameraParameters::PixelFormat format)
```


Set camera image pixel format.

**Parameters**

* const CameraParameters::PixelFormat **format** - Pixel format of the output image to be set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getPixelFormat() {#class_camera_device_1a7eb98b7258304d850cd5b2f6299728c3}
```cpp
virtual Status CameraDevice::getPixelFormat(CameraParameters::PixelFormat &format) const
```


Get camera image pixel format.

**Parameters**

* CameraParameters::PixelFormat& **format** - Pixel format of the output image set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getSupportedPixelFormats() {#class_camera_device_1a7b01831ca40b07d047abb8e26c2080f7}
```cpp
virtual Status CameraDevice::getSupportedPixelFormats(std::vector< CameraParameters::PixelFormat > &formats) const
```


Get supported camera image pixel format.

**Parameters**

* std::vector< CameraParameters::PixelFormat >& **formats** - Vector of PixelFormat supported by the camera device.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setMode() {#class_camera_device_1a4aeb312e3ea2e9b97a5f9934255d498a}
```cpp
virtual Status CameraDevice::setMode(const CameraParameters::Mode mode)
```


Set mode of the camera device.

**Parameters**

* const CameraParameters::Mode **mode** - Camera device mode to be set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getMode() {#class_camera_device_1a3c375f481b80d8c73f34824c46cb60da}
```cpp
virtual Status CameraDevice::getMode(CameraParameters::Mode &mode) const
```


Get mode of the camera device.

**Parameters**

* CameraParameters::Mode& **mode** - Camera device mode that is set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getSupportedModes() {#class_camera_device_1ae0b18c9f04acf1e3a9e02c7f964335c9}
```cpp
virtual Status CameraDevice::getSupportedModes(std::vector< CameraParameters::Mode > &modes) const
```


Get supported modes of the camera device.

**Parameters**

* std::vector< CameraParameters::Mode >& **modes** - Camera device mode that are supported.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setFrameRate() {#class_camera_device_1a969307ab2e83139176e762199f86b97b}
```cpp
virtual Status CameraDevice::setFrameRate(const uint32_t fps)
```


Set frame rate of the camera device.

**Parameters**

* const uint32_t **fps** - Frame rate per second of the camera device to be set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getFrameRate() {#class_camera_device_1a9802d319f82f5b902be109e29253bc9d}
```cpp
virtual Status CameraDevice::getFrameRate(uint32_t &fps) const
```


Get frame rate of the camera device.

**Parameters**

* uint32_t& **fps** - Frame rate per second of the camera device.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getSupportedFrameRates() {#class_camera_device_1a132e700f2e5fd086e62039da38536cf5}
```cpp
virtual Status CameraDevice::getSupportedFrameRates(uint32_t &minFps, uint32_t &maxFps) const
```


Get range of frame rate supported by the camera device.

**Parameters**

* uint32_t& **minFps** - Minimum frame rate per second that can be set.
* uint32_t& **maxFps** - Maximum frame rate per second that can be set.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### setCameraDefinitionUri() {#class_camera_device_1a7e4bca0adbc992262e3e5a14ae7df2eb}
```cpp
virtual Status CameraDevice::setCameraDefinitionUri(const std::string uri)
```


Set URI of the camera definition file for the camera device.

**Parameters**

* const std::string **uri** - String with absolute address of the camera definition file.

**Returns**

&emsp;[Status](class_camera_device.md#class_camera_device_1a6a642ab8816a6e69065dcb32240d58d4) - Status of request.

### getCameraDefinitionUri() {#class_camera_device_1a4d3516539d39ec80f52884acbc3b54a6}
```cpp
virtual std::string CameraDevice::getCameraDefinitionUri() const
```


Get URI of the camera definition file for the camera device. Either the camera device has some predefined/generated URI address OR received by the set function

**Returns**

&emsp;std::string - string URI address of the camera definition file.

### getOverlayText() {#class_camera_device_1a20c1581a6a31fd5c9a71728f39e0be3d}
```cpp
virtual std::string CameraDevice::getOverlayText() const
```


Get text that needs to be overlayed on camera image frames. This may be helpful where some text information can be overlayed on camera images read from the device and displayed to the user. For example, on changing the brighntess parameter to 100, a text like "Brightness = 100" can be displayed on the video that is getting streamed.

**Returns**

&emsp;std::string - string Overlay text.