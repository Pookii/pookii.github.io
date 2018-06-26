#### js和webview交互方法

##### 1.js调用Android原生端方法：

在Android中开启webview debugable设置：

```java
if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.KITKAT) {
    WebView.setWebContentsDebuggingEnabled(true);
}
```

启动webview后，打开Chrome，在chrome://inspect/#devices可以看到已经可以调试的设备。点击设备进入调试界面，注意如果是第一次调试，可能会一直停留在空白页，这是由于初次inspect需要翻墙配置一些东西。



​    