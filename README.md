# Postman Old Install

Postman old version installation packages archive. Please, **use the latest official Postman versions on https://www.postman.com/, if possible.**

**NOTE: These archived installations are WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.**

## 1. For Linux
Download the related GZ files and merge them together:
```
cat Postman-linux-x64-7.34.0.tar.gz_* > Postman-linux-x64-7.34.0.tar.gz
```

## 2. For MacOs
Download the related ZIP files and merge them together:
```
cat Postman-osx-7.34.0.zip_* > Postman-osx-7.34.0.zip
```

## 3. For Windows
Download the related EXE files and merge them together for 64bit:
```
copy /b Postman-win64-7.34.0-Setup.exe_* Postman-win64-7.34.0-Setup.exe
```
or for 32bit:
```
copy /b Postman-win32-7.34.0-Setup.exe_* Postman-win32-7.34.0-Setup.exe
```

## Apendix A. Commands used for split
```
md5sum Postman-osx-7.34.0.zip > Postman-osx-7.34.0.zip.md5
md5sum Postman-linux-x64-7.34.0.tar.gz > Postman-linux-x64-7.34.0.tar.gz.md5
md5sum Postman-win32-7.34.0-Setup.exe > Postman-win32-7.34.0-Setup.exe.md5
md5sum Postman-win64-7.34.0-Setup.exe > Postman-win64-7.34.0-Setup.exe.md5

sha256sum Postman-osx-7.34.0.zip > Postman-osx-7.34.0.zip.sha256
sha256sum Postman-linux-x64-7.34.0.tar.gz > Postman-linux-x64-7.34.0.tar.gz.sha256
sha256sum Postman-win32-7.34.0-Setup.exe > Postman-win32-7.34.0-Setup.exe.sha256
sha256sum Postman-win64-7.34.0-Setup.exe > Postman-win64-7.34.0-Setup.exe.sha256

split -b 24M -d Postman-osx-7.34.0.zip Postman-osx-7.34.0.zip_
split -b 24M -d Postman-linux-x64-7.34.0.tar.gz Postman-linux-x64-7.34.0.tar.gz_
split -b 24M -d Postman-win32-7.34.0-Setup.exe Postman-win32-7.34.0-Setup.exe_
split -b 24M -d Postman-win64-7.34.0-Setup.exe Postman-win64-7.34.0-Setup.exe_
```


