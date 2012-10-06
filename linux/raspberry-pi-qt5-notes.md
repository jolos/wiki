# Troubleshooting for running qt5 on raspberry pi :

- the linaro toolchain is 32bit, make sure you have the 32bit versions of all the libraries ( if you're running on 64bit )
- if you have troubles with getting deployment to remote linux right, try qt creator 2.6 beta. Somehow I could not get this configured with earlier versions.
- make sure LD_LIBRARY_PATH is set when compiling in qtcreator
- make sure that you're image is mounted while compiling in qt creator
- if not all files get deployed to the rpi, try disabling incremental deployments
