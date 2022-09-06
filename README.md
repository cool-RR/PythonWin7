# Unofficial Python Installers for Windows 7 and Windows Server 2003 R2

Officially, Python 3.9 and 3.10 are not supported on Windows 7 and Windows Server 2003 R2. Here, you can obtain unofficial Windows installers that bring back support for these older Windows versions. 

For each Python version, this repository includes the following.
- 64-bit executable installer (e.g. python-3.9.0-amd64-full.exe)
- 32-bit executable installer (e.g. python-3.9.0-full.exe)
- 64-bit embeddable zip file (e.g. python-3.9.0-embed-amd64.zip)
- 32-bit embeddable zip file (e.g. python-3.9.0-embed-win32.zip)
- 64-bit NuGet package (e.g. python.3.9.0.nupkg)
- 32-bit NuGet package (e.g. pythonx86.3.9.0.nupkg)

For the more technical among you, these installers were built from the source distributions published at https://www.python.org/downloads/source/, with the following modifications.
- Include the file `api-ms-win-core-path-l1-1-0.dll` in the distribution. This file was obtained from https://github.com/nalexandru/api-ms-win-core-path-HACK and is necessary for Python to run on older Windows versions.
- Create full installers that include debugging symbols and debug binaries without needing to download them.
- Allow the installer to proceed on Windows 7 and Windows Server 2003 R2.

**The files are provided "as is" without warranty or support of any kind.**
