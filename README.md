# Maxim 

> A Kotlin implementation of Monkey TEST(Non-Stub) for Android that runs on Simulator/Android devices. 

## 1. Requirements

- Android 6.0

## 2. Setup

- adb push framework.jar /sdcard
- adb push monkey.jar /sdcard

## 3. Usage 

Maxim can be either started with adb command line. 

- adb shell CLASSPATH=/sdcard/monkey.jar:/sdcard/framework.jar exec app_process /system/bin tv.panda.test.monkey.Monkey -p com.panda.videoliveplatform --uiautomatordfs 5000

### 3.1 Args

--uiautomatordfs    monkey use DFS algorithm .  About 5 action per second.

--uiautomator         monkey use AccessibilityService resolve tree node and random choose.  About 10-15 action per second.

other args is same to Android Monkey


