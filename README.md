# Evaluation of Neutralinojs

[Neutralinojs](https://github.com/neutralinojs/neutralinojs) framework was evaluvated in comparison with Electron and NW.js considering disk consumption, memory consumption, easiness of development workflow and portability.

### Sample applications

Simple `Hello World` type application is used in each framework on Linux and Windows for the evaluation.

<img src="media/linux-apps.JPG">
Figure 1: Sample cross-platform apps written using Electron, NW.js and Neutralino respectively on Linux.<br/><br/>

<img src="media/win-apps.JPG">
Figure 2: Sample cross-platform apps written using Electron, NW.js and Neutralino respectively on Windows.

#### OS details

- Ubuntu 18.04.1 LTS
- Windows 10 Enterprise


## 1. Disk Consumption

### Node Webkit

#### Linux

```
Zipped SDK size                   95.8 MB
Project Size                      1 KB
Application bundle                97.2 MB
Application bundle (zipped)       36.9 MB
File count of project             5         
```

#### Windows

```
Zipped SDK size                   72.7 MB
Project size                      2 KB
Application bundle                78.1 MB
Application bundle (zipped)       32.3 MB
File count of project             5
```

### Electron

#### Linux

```
Build package                     51.53 MB
node_modules count                147 
File count of project             1539
Project size                      136.4 MB
Application bundle                128.6 MB
Application bundle (zipped)       51.5 MB
```

#### Windows 

```
Build package                     53.16 MB
node_modules count                180 
project file count                1368
total project size                125 MB
application bundle                118 MB
application bundle zipped         50.4 MB
```


### Neutralinojs


#### Linux

```
Portable SDK size                 5.8 MB
Portable SDK size (zipped)        1.1 MB
File count                        11
```
#### Windows

```
Portable SDK size                 5.53 MB
portable SDK size zipped          1.01 MB
File count                        11
```
SDK and application bundle are similar things in Neutralino. We will be introducing a application builder CLI soon!.

See [proof](https://github.com/neutralinojs/evaluation/tree/master/disk/proof) directory for sample sources and binary releases.

## 2. Memory consumption

### NW.js

```
Linux                           ~ 40 - 42 MB
Windows                         ~ 40 - 45 MB
```

### Electron

```
Linux                           ~ 62 - 65 MB
Windows                         ~ 45 - 50 MB
```

### Neutralinojs

```
Linux                           ~ 8 - 9 MB
Windows                         ~ 6 - 7 MB  
```

## 3. Easiness Development Workflow

### Electron

<div align="center">
  <img src="media/dev-el.JPG"/>
</div>

### NW.js

<div align="center">
  <img src="media/dev-nwjs.JPG"/>
</div>

### Neutralino

<div align="center">
  <img src="media/dev-njs.JPG"/>
</div>

### Neutralino Debugging

Neutralino app is served via a socket. Therefore debugging can be done using a web browser.

<img src="media/debug-njs.JPG">
Figure 3: Debugging a Neutralino based app using Google Chrome.<br/><br/>

## 4. Conclusion

According to the results of this expertiment Neutralino can be used as a lightweight alternative for Electron and NW.js. Furthermore another experiment needs to be done by using somewhat large cross platform application such as [draw.io](https://github.com/jgraph/drawio). There are some drawbacks such as Windows edition is based on IE etc.
