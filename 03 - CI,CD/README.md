![image](./setup.png)
# CI / CD
## Ruby
### 설치
```shell
brew install rbenv ruby-build
```
```shell
rbenv install -l
```
```shell
rbenv install <version>
```
```shell
rbenv global <version>
```
<br/>

### 환경 변수 설정
```shell
vi ~/.zshrc
```
```shell
# rbenv
[[ -d ~/.rbenv  ]] && \
export PATH=${HOME}/.rbenv/bin:${PATH} && \
eval "$(rbenv init -)"
```
```shell
source ~/.zshrc
```
<br/>
<br/>

## Fastlane
### 설명
### **설명**
Bundler 는 Ruby 프로젝트에 알맞은 Gem 과 버전을 추적할 수 있게 도와주는 라이브러리이다.<br/>
Gem 은 Ruby 프로젝트에서의 라이브러리이다.<br/>
Gemfile 은 Gem 을 등록하는 방식으로 의존성을 관리해주는 파일이다.<br/>
<br/>

### 설치
```shell
gem install bundler
```
<br/>

### fastlane 폴더 생성
```shell
mkdir ~/AndroidStudioProjects/<project>/fastlane
```
<br/>

### .Gemfile 생성
```shell
touch ~/AndroidStudioProjects/<project>/.Gemfile
```
````shell
source "https://rubygems.org"

gem "fastlane"
plugins_path = File.join(File.dirname(__FILE__), 'fastlane', 'Pluginfile')
eval_gemfile(plugins_path) if File.exist?(plugins_path)
````
<br/>

### 설정
```shell
bundle install
```
```shell
bundle update
```
```shell
fastlane init
```