BaiduGeolocationPlugin
======================

Cordova 百度定位插件，兼容 w3c 的 geolocation 标准，解决中国大陆手机无法定位的问题。使用前需要在百度申请应用。

使用方法
--------

### window.geolocation.getCurrentPosition(success, error, [options]);
获取当前位置
```
var options = {
  enableHighAccuracy: true,  // 是否使用 GPS
  maximumAge: 30000,         // 缓存时间
  timeout: 27000             // 超时时间
}
```

### window.geolocation.watchPosition(success, error, [options]);
持续追踪位置变更

### window.geolocation.clearWatch(watchId);
清楚位置追踪

安装方法
-------

```
cordova plugin add https://github.com/gengen1988/BaiduGeolocationPlugin.git --variable ACCESS_KEY={{your access key}}
```
