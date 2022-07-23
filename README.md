# Image Compressor

The Android image compression library image compressor is small and effective. With very little or no image quality degradation, a compressor enables you to reduce the size of large photos into smaller photos.

# How to
To get a Git project into your build:
## Gradle
` Step 1:` Add it in your **root build.gradle**  at the end of repositories:
```kotlin
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

`Step 2:` Add the dependency in your **project build.gradle**
```kotlin
dependencies {
	        implementation 'com.github.vinodbaste:ImageCompressor:1.0.0'
	}
```
# Let's compress the image size!
#### Compress Image File at the specified `imagePath`
```kotlin
ImageCompressUtils.compressImage(
            context = this,
            imagePath = "actualImagePath",
            imageName = "imageName",
            imageQuality = 50
        )
```
**imageQuality** is set to `50` by default.

#### Compress Image File at the specified `imagePath` and return the `compressed ImagePath`
```kotlin
val compressedImagePath = ImageCompressUtils.compressImage(
            context = this,
            imagePath = "actualImagePath",
            imageName = "imageName",
            imageQuality = 50
        )
```



