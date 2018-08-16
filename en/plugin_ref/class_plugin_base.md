# PluginBase Class Reference
`#include: PluginBase.h`

----


The [PluginBase](class_plugin_base.md) is base class for plugins. Plugins are factories for a class of CameraDevices. For example - PluginV4l2 creates [CameraDevice](class_camera_device.md) object for V4L2 cameras discovered in the system. Plugins that gets compiled will self-register on execution using static initialization. PluginManager maintains a table of Plugins and camera devices associated with each Plugin. To add support for custom type of camera, implement a custom Plugin derived from [PluginBase](class_plugin_base.md). This custom Plugin will create custom [CameraDevice](class_camera_device.md). 


## Public Member Functions


Type | Name | Description
---: | --- | ---
&nbsp; | [~PluginBase](#class_plugin_base_1acd9059487943c31e2a7cf38efc0119ef) () |
std::vector< std::string > | [getCameraDevices](#class_plugin_base_1a6699342e4ebaf1405365582fd641a7ea) ()=0 |
std::shared_ptr< [CameraDevice](class_camera_device.md) > | [createCameraDevice](#class_plugin_base_1a7c71a01d88b12c7b0422a1c4926b7758) (std::string deviceID)=0 |

## Static Public Member Functions


Type | Name | Description
---: | --- | ---
std::vector< [PluginBase](class_plugin_base.md) * > & | [getPlugins](#class_plugin_base_1a17e47c421f85dc3711638ef698d279ec) () |

## Protected Member Functions


Type | Name | Description
---: | --- | ---
&nbsp; | [PluginBase](#class_plugin_base_1ab59f1c42801522322ebf1dd6a0d5d0b8) () |


## Constructor & Destructor Documentation


### ~PluginBase() {#class_plugin_base_1acd9059487943c31e2a7cf38efc0119ef}
```cpp
virtual PluginBase::~PluginBase()
```


Destructor. Erases itself from the list.

### PluginBase() {#class_plugin_base_1ab59f1c42801522322ebf1dd6a0d5d0b8}
```cpp
PluginBase::PluginBase()
```


Constructor. Self-registers by adding itself to the list.

## Member Function Documentation


### getCameraDevices() {#class_plugin_base_1a6699342e4ebaf1405365582fd641a7ea}
```cpp
virtual std::vector<std::string> PluginBase::getCameraDevices()=0
```


Get the list of camera devices discovered by plugin.

**Returns**

&emsp;std::vector< std::string > - Vector of names(ID) of camera devices.

### createCameraDevice() {#class_plugin_base_1a7c71a01d88b12c7b0422a1c4926b7758}
```cpp
virtual std::shared_ptr<CameraDevice> PluginBase::createCameraDevice(std::string deviceID)=0
```


Create a [CameraDevice](class_camera_device.md).

**Parameters**

* std::string **deviceID** - Camera device identifier(name)

**Returns**

&emsp;std::shared_ptr< [CameraDevice](class_camera_device.md) > - Pointer to [CameraDevice](class_camera_device.md) object created or nullptr on failure

### getPlugins() {#class_plugin_base_1a17e47c421f85dc3711638ef698d279ec}
```cpp
static std::vector<PluginBase *>& PluginBase::getPlugins()
```


Get the list of plugin objects.

**Returns**

&emsp;std::vector< [PluginBase](class_plugin_base.md) * > & - Reference to vector of plugin object.