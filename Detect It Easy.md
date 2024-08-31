# Detect It Easy



> - ### [DOWNLOAD **RELEASE**](https://github.com/horsicq/DIE-engine/releases)
>
>   
>
> - ### [DOWNLOAD LATEST **BETA**](https://github.com/horsicq/Detect-It-Easy/releases/tag/Beta)
>
>   
>
> - #### [DIE API Library (for developers)](https://github.com/horsicq/die_library)
>
>   

- Changelog: https://github.com/horsicq/Detect-It-Easy/blob/master/changelog.txt

You can help with translation: https://github.com/horsicq/XTranslation

[![alt text](https://github.com/horsicq/Detect-It-Easy/raw/master/docs/1.png)](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/1.png) [![alt text](https://github.com/horsicq/Detect-It-Easy/raw/master/docs/2.png)](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/2.png) [![alt text](https://github.com/horsicq/Detect-It-Easy/raw/master/docs/3.png)](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/3.png) [![alt text](https://github.com/horsicq/Detect-It-Easy/raw/master/docs/4.png)](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/4.png) [![alt text](https://github.com/horsicq/Detect-It-Easy/raw/master/docs/5.png)](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/5.png)

**Detect It Easy**, or abbreviated "DIE" is a program for determining types of files.

DIE is a cross-platform application, apart from Windows version there are also available versions for Linux and Mac OS.

Many programs of the kind (PEID, PE tools) allow to use third-party signatures. Unfortunately, those signatures scan only bytes by the pre-set mask, and it is not possible to specify additional parameters. As the result, false triggering often occur. More complicated algorithms are usually strictly set in the program itself. Hence, to add a new complex detect one needs to recompile the entire project. No one, except the authors themselves, can change the algorithm of a detect. As time passes, such programs lose relevance without the constant support.

**Detect It Easy** has totally open architecture of signatures. You can easily add your own algorithms of detects or modify those that already exist. This is achieved by using scripts. The script language is very similar to JavaScript and any person, who understands the basics of programming, will understand easily how it works. Possibly, someone may decide the scripts are working very slow. Indeed, scripts run slower than compiled code, but, thanks to the good optimization of Script Engine, this doesn't cause any special inconvenience. The possibilities of open architecture compensate these limitations.

DIE exists in three versions. Basic version ("die"), Lite version ("diel") and console version ("diec"). All the three use the same signatures, which are located in the folder "db". If you open this folder, nested sub-folders will be found ("Binary", "PE" and others). The names of sub-folders correspond to the types of files. First, DIE determines the type of file, and then sequentially loads all the signatures, which lie in the corresponding folder. Currently the program defines the following types:

- MSDOS executable files MS-DOS
- PE executable files Windows
- ELF executable files Linux
- MACH executable files Mac OS
- Binary all other files

# Installing



### Using installation packages



- Windows: [die](https://community.chocolatey.org/packages/die) on Chocolatey (Thanks [**chtof**](https://github.com/chtof) 和 [**Rob Reynolds**](https://github.com/ferventcoder))
- Parrot OS: Package name **detect-it-easy** (Thanks [**Nong Hoang Tu**](https://github.com/dmknght))
- Arch Linux: Aur package [detect-it-easy-git](https://aur.archlinux.org/packages/detect-it-easy-git/) (Thanks [**Arnaud Dovi**](https://github.com/class101))
- [REMnux](https://remnux.org/): (Thanks [**REMnux team**](https://twitter.com/REMnux/status/1401935989266919426))
- openSUSE: [detect-it-easy](https://build.opensuse.org/package/show/home:mnhauke/detect-it-easy) (Thanks Martin Hauke)

### Build from source



Build instructions can be found in [BUILD.md](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/BUILD.md)。

### Docker install



You can also run DIE with [Docker](https://www.docker.com/community-edition)! Of course, this requires that you have git and Docker installed.

```
git clone --recursive https://github.com/horsicq/Detect-It-Easy
cd Detect-It-Easy/
docker build . -t horsicq:diec
```



# Usage



### detect-it-easy has 3 variants



- `die` GUI version
- `diec` console version
- `diel` GUI lite version

Detailed usage instructions can be found in [RUN.md](https://github.com/horsicq/Detect-It-Easy/blob/master/docs/RUN.md)。