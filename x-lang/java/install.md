通过homebrew安装，目前主流版本还是1.8，所以这里安装1.8版本
```sh
brew tap caskroom/versions
brew cask install java8
```

查看安装版本
```sh
java -version
```

修改idea里jdk配置
```
File -> Project Structure -> Project Settings -> Project -> Project SDK
File -> Project Structure -> Platform Settings -> SDKs -> +
```