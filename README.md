# Demo170924
```java
// Check for POST_NOTIFICATIONS permission for Android Tiramisu (API level 33)
if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.TIRAMISU) {
    if (ContextCompat.checkSelfPermission(MainActivity.this,
            android.Manifest.permission.POST_NOTIFICATIONS) != PackageManager.PERMISSION_GRANTED) {

        ActivityCompat.requestPermissions(MainActivity.this,
                new String[]{android.Manifest.permission.POST_NOTIFICATIONS}, 101);
    }
}
