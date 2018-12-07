# Evaluation of Neutralinojs

Neutralinojs framework was evaluvated in comparison with Electron and NW.js considering disk consumption, memory consumption, easiness of development workflow and portability.

### Sample applications

Simple `Hello World` type application is used in each framework on Linux and Windows for the evaluation.


## 1. Disk Usage

### Node Webkit

#### Linux

```
zipped sdk size                   95.8 MB
total project size                1 KB
application bundle                97.2 MB
application bundle zipped         36.9 MB
project file count                5         
```

#### Windows

```
zipped sdk size                   72.7 MB
total project size                2 KB
application bundle                78.1 MB
application bundle zipped         32.3 MB
project file count                5
```

### Electron

#### Linux

```
build package                     51.53 MB
node_modules count                147 
project file count                1539
total project size                136.4 MB
application bundle                128.6 MB
application bundle zipped         51.5 MB
```

#### Windows 

```
build package                     53.16 MB
node_modules count                180 
project file count                1368
total project size                125 MB
application bundle                118 MB
application bundle zipped         50.4 MB
```


### Neutralinojs


#### Linux

```
portable sdk size                 5.8 MB
portable sdk size zipped          1.1 MB
file count                        11
```
#### Windows

```
portable sdk size                 5.53 MB
portable sdk size zipped          1.01 MB
file count                        11
```
sdk and application bundle are similar in njs

See [proof](https://github.com/neutralinojs/evaluation/tree/master/disk/proof) directory for sample `Hello Wolrd` source and binary releases.

# Memory consumption

Physical memory consumption comparison with simple `Hello World` application on Linux and Windows.

## NW.js

```
Linux                           ~ 40 - 42 MB
Windows                         ~ 40 - 45 MB
```

## Electron

```
Linux                           ~ 62 - 65 MB
Windows                         ~ 45 - 50 MB
```

## Neutralinojs

```
Linux                           ~ 8 - 9 MB
Windows                         ~ 6 - 7 MB  
```
