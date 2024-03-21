# OtpViewDemo

[![](https://jitpack.io/v/arnab-kundu/otpviewLibrary.svg)](https://jitpack.io/#arnab-kundu/otpviewLibrary)

## How to use

Step 1. Add it in your root build.gradle at the end of repositories(for Gradle 6.7 or lower):

```groovy
allprojects {
    repositories {
        //...
        maven { url 'https://jitpack.io' }
    }
}
```

Or For API 33(Gradle 6.8 or higher) in settings.gradle

```groovy
dependencyResolutionManagement {
    //...
    repositories {
        //...
        maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency

```groovy
dependencies {
    implementation 'com.github.arnab-kundu:otpviewLibrary:1.0.9'
}
```

Step 3. Use this below xml code in your layout file to use OtpView
```xml
<com.arnab.otpview.OtpTextView
    android:id="@+id/pincodeTextFieldView"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:textColor="@color/black"
    app:bar_active_color="@color/purple_200"
    app:bar_enabled="true"
    app:bar_error_color="@color/red"
    app:bar_height="2dp"
    app:bar_inactive_color="@android:color/transparent"
    app:bar_margin_bottom="5dp"
    app:bar_margin_left="5dp"
    app:bar_margin_right="5dp"
    app:bar_success_color="@android:color/holo_green_light"
    app:box_margin="@dimen/registerPinCodeBoxMargin"
    app:height="40dp"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:length="6"
    app:otp=""
    app:otp_box_background="@drawable/white_border_background"
    app:otp_text_size="24dp"
    app:width="@dimen/registerPinCodeBoxWidth" />
```


## :hammer_and_wrench: Build Tool

- Android Studio Iguana | 2023.2.1
- Minimum SDK version: 24
- Target SDK version: 34
- JDK version: 17
