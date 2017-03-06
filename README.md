# CameraPermissionCompat
Android相机权限检测兼容

```
CameraPermissionCompat.checkCameraPermission(this, new CameraPermissionCompat.OnCameraPermissionListener() {
        @Override
        public void onGrantResult(boolean granted) {
            Log.d(TAG,"权限--------->"+granted);
        }
});
```
        
```
 @Override
public void onRequestPermissionsResult(int requestCode, @NonNull String[] permissions, @NonNull int[] grantResults) {
    super.onRequestPermissionsResult(requestCode, permissions, grantResults);
    CameraPermissionCompat.onRequestPermissionsResult(this,requestCode,permissions,grantResults);
}
```
