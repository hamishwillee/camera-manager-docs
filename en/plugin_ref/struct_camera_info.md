# CameraInfo Struct Reference
`#include: CameraDevice.h`

----


The [CameraInfo](struct_camera_info.md) structure is used to hold the camera device information. 


## Data Fields


uint8_t [vendorName](#struct_camera_info_1a23844d6d1740e872be7a06eb5884f98d)  -

uint8_t [modelName](#struct_camera_info_1a91c9e671b1556901b8b1020d77d2c3b4)  -

uint32_t [firmware_version](#struct_camera_info_1a3366ea617e7f45ed01cdce563098c071)  -

float [focal_length](#struct_camera_info_1a69ec85b6e83d7eb0b77e25a37ecffb7d)  -

float [sensor_size_h](#struct_camera_info_1a88980b012519b28b6bf91103fd502599)  -

float [sensor_size_v](#struct_camera_info_1ab8db2cb99894a2b12223e523135484e3)  -

uint16_t [resolution_h](#struct_camera_info_1af5e5eaaf87f126ac5d498b736255a31c)  -

uint16_t [resolution_v](#struct_camera_info_1aa338fc7bb832aa53c9a17d14e187e629)  -

uint8_t [lens_id](#struct_camera_info_1ae9a7a845d3166a59b7667e3c8d2e4b3c)  -

uint32_t [flags](#struct_camera_info_1adb7045c02bbe38ec186bca3083a53456)  -

uint16_t [cam_definition_version](#struct_camera_info_1a4d63a081b79c84472566c2a52d7ff1f0)  -

char [cam_definition_uri](#struct_camera_info_1a515ab924ca351d412fbdacd566a3b50f)  -


## Field Documentation


### vendorName {#struct_camera_info_1a23844d6d1740e872be7a06eb5884f98d}

```cpp
uint8_t CameraInfo::vendorName[32]
```


Name of the camera device vendor.

### modelName {#struct_camera_info_1a91c9e671b1556901b8b1020d77d2c3b4}

```cpp
uint8_t CameraInfo::modelName[32]
```


Name of the camera device model.

### firmware_version {#struct_camera_info_1a3366ea617e7f45ed01cdce563098c071}

```cpp
uint32_t CameraInfo::firmware_version
```


Firmware version.

### focal_length {#struct_camera_info_1a69ec85b6e83d7eb0b77e25a37ecffb7d}

```cpp
float CameraInfo::focal_length
```


Focal length.

### sensor_size_h {#struct_camera_info_1a88980b012519b28b6bf91103fd502599}

```cpp
float CameraInfo::sensor_size_h
```


Sensor size horizontol.

### sensor_size_v {#struct_camera_info_1ab8db2cb99894a2b12223e523135484e3}

```cpp
float CameraInfo::sensor_size_v
```


Sensor size vertical.

### resolution_h {#struct_camera_info_1af5e5eaaf87f126ac5d498b736255a31c}

```cpp
uint16_t CameraInfo::resolution_h
```


Resolution horizontol.

### resolution_v {#struct_camera_info_1aa338fc7bb832aa53c9a17d14e187e629}

```cpp
uint16_t CameraInfo::resolution_v
```


Resolution vertical.

### lens_id {#struct_camera_info_1ae9a7a845d3166a59b7667e3c8d2e4b3c}

```cpp
uint8_t CameraInfo::lens_id
```


Lens ID.

### flags {#struct_camera_info_1adb7045c02bbe38ec186bca3083a53456}

```cpp
uint32_t CameraInfo::flags
```


Flags

### cam_definition_version {#struct_camera_info_1a4d63a081b79c84472566c2a52d7ff1f0}

```cpp
uint16_t CameraInfo::cam_definition_version
```


Camera Definition file version

### cam_definition_uri {#struct_camera_info_1a515ab924ca351d412fbdacd566a3b50f}

```cpp
char CameraInfo::cam_definition_uri[140]
```


Camera Definition file URI address