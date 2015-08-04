# BrokenCocoapods
Swift fails to code complete when using a symlink to specify the path to a Development Pod

# How to reproduce

Create a 'components' directory where the development pod will be stored and git clone a pod written in Swift

```
mkdir ~/Desktop/components
cd ~/Desktop/components && git clone https://github.com/Alamofire/Alamofire.git 
```

Create a symlink in the DemoProject base directory to the 'components' directory we just created

Ex:
```
ln -s ~/Desktop/components .
```

Pod install

```
pod install
```

** When attempting to edit the Alamofire development pod swift does not syntax highlight correctly **
