![image](./setup.png)
# Android
## Android Studio
### 설치
[Android Studio 및 앱 도구 다운로드](https://developer.android.com/studio?hl=ko)<br/>
<br/>

### 환경 변수 설정
```shell
vi ~/.zshrc
```
```shell
# Android
export ANDROID_HOME=/Users/mg.yang/Library/Android/sdk
export ANDROID_ADB=$ANDROID_HOME/platform-tools
export PATH=$PATH:$ANDROID_SDK:$ANDROID_ADB
```
```shell
source ~/.zshrc
```
<br/>
<br/>

## JDK
### 설치
```shell
brew install openjdk@21
```
<br/>

### 환경 변수 설정
```shell
vi ~/.zshrc
```
```shell
# JDK
export JAVA_HOME="/opt/homebrew/opt/openjdk@21"
export PATH=$JAVA_HOME/bin:$PATH
```
```shell
source ~/.zshrc
```