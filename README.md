This a sub-repo of [Neard project](https://github.com/crazy-max/neard) involving MySQL binary bundles.

## Installation

* Download and install [Neard](https://github.com/crazy-max/neard).
* If you already have installed Neard, stop it.
* Download [a MySQL bundle](#download).
* Use a file archiver that supports [7z format](http://www.7-zip.org/7z.html) like [7zip](http://www.7-zip.org/) and extract the archive in `neard\bin\mysql\`.

Directory structure example :
```
[-] neard
 | [-] bin
 |  | [-] mysql
 |  |  | [-] mysql5.5.24
 |  |     | neard.conf
 |  |  | [-] mysql5.6.27
 |  |     | neard.conf
 ```

* Start Neard.
* Switch to the MySQL version you have extracted on Neard :

![](https://raw.github.com/crazy-max/neard-bin-mysql/master/img/switchVersion-20151214.png)

## Download

![](https://raw.github.com/crazy-max/neard-bin-mysql/master/img/star-20151214.png) : Default bundle on Neard.

### 5.5

|                  | MySQL release date | Neard release | Download |
| ---------------- |:------------------:|:-------------:|:--------:|
| **MySQL 5.5.24** ![](https://raw.github.com/crazy-max/neard-bin-mysql/master/img/star-20151214.png) | 2012/05/07 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.5.24-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.5.24-r1.zip) |
| **MySQL 5.5.44** | 2015/05/29 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.5.44-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.5.44-r1.zip) |
| **MySQL 5.5.46** | 2015/09/30 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.5.46-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.5.46-r1.zip) |
| **MySQL 5.5.49** | 2016/04/11 | [r2](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r2) | [neard-mysql-5.5.49-r2.7z](https://github.com/crazy-max/neard-bin-mysql/releases/download/r2/neard-mysql-5.5.49-r2.7z) |

### 5.6

|                  | MySQL release date | Neard release | Download |
| ---------------- |:------------------:|:-------------:|:--------:|
| **MySQL 5.6.12** | 2013/06/03 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.6.12-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.6.12-r1.zip) |
| **MySQL 5.6.25** | 2015/05/29 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.6.25-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.6.25-r1.zip) |
| **MySQL 5.6.27** | 2015/09/30 | [r1](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r1) | [neard-mysql-5.6.27-r1.zip](https://github.com/crazy-max/neard-bin-mysql/releases/download/r1/neard-mysql-5.6.27-r1.zip) |
| **MySQL 5.6.30** | 2016/04/11 | [r2](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r2) | [neard-mysql-5.6.30-r2.7z](https://github.com/crazy-max/neard-bin-mysql/releases/download/r2/neard-mysql-5.6.30-r2.7z) |

### 5.7

|                  | MySQL release date | Neard release | Download |
| ---------------- |:------------------:|:-------------:|:--------:|
| **MySQL 5.7.12** | 2016/04/11 | [r3](https://github.com/crazy-max/neard-bin-mysql/releases/tag/r3) | [neard-mysql-5.7.12-r3.7z](https://github.com/crazy-max/neard-bin-mysql/releases/download/r3/neard-mysql-5.7.12-r3.7z) |

## Sources

* https://dev.mysql.com/

## Contribute

If you want to contribute to this bundle and create new bundles, you have to download [neard-dev](https://github.com/crazy-max/neard-dev) in the parent folder of the bundle.
Directory structure example :

```
[-] neard-dev
 | [-] build
 |  |  | build-commons.xml 
[-] neard-bin-mysql
 |  | build.xml
```

To create a new bundle :
* Do not forget to increment the `build.release` in the `build.properties` file.
* If you want you can change the `build.path` (default `C:\neard-build`).
* Open a command prompt in your bundle folder and call the Ant target `release` : `ant release`.
* Upload your release on a file hosting system like [Sendspace](https://www.sendspace.com/).
* Create an [issue on Neard repository](https://github.com/crazy-max/neard/issues) to integrate your release.

## Issues

Issues must be reported on [Neard repository](https://github.com/crazy-max/neard/issues).<br />
Please read [Found a bug?](https://github.com/crazy-max/neard#found-a-bug) section before reporting an issue.
