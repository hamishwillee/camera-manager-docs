# CameraData Struct Reference
`#include: CameraDevice.h`

----


The [CameraData](struct_camera_data.md) structure is used to hold the camera image data and its meta-data. 


## Data Fields


uint32_t [sec](#struct_camera_data_1a944312a3b94a797f4da268926ebf2d87) = 0 -

uint32_t [nsec](#struct_camera_data_1ad92486b3905bdcad0374d8c4e8f8afd2) = 0 -

uint32_t [width](#struct_camera_data_1a0df0e738ee1638d23d9a629ae95eadaa) = 0 -

uint32_t [height](#struct_camera_data_1a837da253b1ffb21afdea3c7172085b2c) = 0 -

uint32_t [stride](#struct_camera_data_1a9c9bf37ce671528406695b5ed449d8ee) = 0 -

void * [buf](#struct_camera_data_1a1aefa413e1818f8b64a0f8776a6a3104) = nullptr -

size_t [bufSize](#struct_camera_data_1a935d754a6ec486c3111d114ff619faa3) = 0 -


## Field Documentation


### sec {#struct_camera_data_1a944312a3b94a797f4da268926ebf2d87}

```cpp
uint32_t CameraData::sec = 0
```


system time in sec.

### nsec {#struct_camera_data_1ad92486b3905bdcad0374d8c4e8f8afd2}

```cpp
uint32_t CameraData::nsec = 0
```


system time in nano sec.

### width {#struct_camera_data_1a0df0e738ee1638d23d9a629ae95eadaa}

```cpp
uint32_t CameraData::width = 0
```


width of the image.

### height {#struct_camera_data_1a837da253b1ffb21afdea3c7172085b2c}

```cpp
uint32_t CameraData::height = 0
```


height of the image.

### stride {#struct_camera_data_1a9c9bf37ce671528406695b5ed449d8ee}

```cpp
uint32_t CameraData::stride = 0
```


stride.

### buf {#struct_camera_data_1a1aefa413e1818f8b64a0f8776a6a3104}

```cpp
void* CameraData::buf = nullptr
```


buffer address.

### bufSize {#struct_camera_data_1a935d754a6ec486c3111d114ff619faa3}

```cpp
size_t CameraData::bufSize = 0
```


buffer size.