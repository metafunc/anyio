# AnyIO

![AnyIO](https://img.shields.io/badge/POSIX-AnyIO-blue?style=flat-square)
![Version](https://img.shields.io/github/v/release/metafunc/anyio?include_prereleases&sort=date&display_name=release&style=flat-square)
![Stars](https://img.shields.io/github/stars/metafunc/anyio?style=flat-square)
![Forks](https://img.shields.io/github/forks/metafunc/anyio?style=flat-square)
![Downloads](https://img.shields.io/github/downloads/metafunc/anyio/total?style=flat-square)

<img align="right" width="150px" src="https://raw.githubusercontent.com/metafunc/anyio/refs/heads/main/assets/images/anyio-logo.png" />

[AnyIO][anyio dev], It means `Anywhere can create I/O`, and fully establishes *POSIX operations*, even *FS operations*, on any storage method. Even in harsh file reading and writing environments, it is easy to cope with and build various high-performance services.

# Features
+ 👌 The required are as low as *Can only write the entire file at once (w+)* and *Can only read the entire file at once*
+ 🔒 Provides a comprehensive multi terminal **Read-Write Lock Mechanism** based solely on file read and write
+ 📒 Provided a comprehensive **Distributed System** based solely on file read and write operations
+ 🚀 Maintaining **High-Performance** despite storing *millions of files* and *100, 0000 GB*
+ 🔁 **Quickly Refresh Outdated Cache** and **Quickly Pull the Required Cache** *(means faster re-reading speed after recovery)*
+ 🔄 Maintain **Synchronous High-Performance** in complex environments
+ 📶 Efficiently achieving **Full I/O Functionality** in the *absence of complete I/O functionality*

# Projects
## IOCovalent
API Class

## IOElectron
This project maintains a complete set of **Distributed Task Syntax** and **Distributed System**, aiming to hand over transaction tasks to each connected device for execution, while ensuring smooth operation and avoiding mutual interference.

## IOProton
This project aggregates the functionality provided by IOCovalent and further processes it into I/O operations that can be executed by the **POSIX** standard.

+ Simple and efficient **Metadata**
+ Strict **Locking Mechanism**
+ Expanded complete I/O functionality

| Object Type | Operation Type | Descrption / Content |
| --- | --- | --- |
| File | Read | `Seek` `All` `Line` `Stream` |
|  | Write | `Seek` `All` `Line` `Stream` |
|  | Rename |  |
|  | Create |  |
|  | Delete | Delete the pointed file and all links pointing to the file |
|  | Move |  |
|  | Copy |  |
|  | Meta data | `Last editing datetime` `Creation datetime` `File size` <br /> `CRC32` `MD5` `SHA256` `SHA512` `UUID` `Path` `Versions` |
| Directory | List | `Subfolders` `Recursive Subfolders` |
|  | Create | `Single` `Multiple` |
|  | Delete | Delete the pointed directory and all links pointing to the directory |
|  | Rename |  |
|  | Copy |  |
|  | Meta data | `Last editing datetime` `Creation datetime` `Directory size` <br /> `UUID` `Path` |
| Link | Bind / Create | Point to an existing file or directory |
|  | Relink | Modify the file or directory pointed to |
|  | Move |  |
|  | Rename |  |
|  | Move |  |
|  | Delete |  |
|  | Meta data | Meta data of the file or directory pointed to |

## IONeutron
The complete **File System** has been implemented on IOProton's API, with functional extensions and objective performance optimizations for various operations, making it a hero in **Saving Space** and **Reducing Consumption**.

+ Maintain file index (for **Fuzzy Search** or speed-up)
+ Expand the properties that files can hold and allow customization
+ Automatically handle index redirection to **Improve the Speed** of operations such as `move`, `copy`, `rename`, and `delete`
+ Process FS metadata with a better solution instead of using the original solution
+ Add predictive strategies to improve the speed of `read`, `pull`, and other operations

  [anyio dev]: https://anyio.metafunc.dev/9
