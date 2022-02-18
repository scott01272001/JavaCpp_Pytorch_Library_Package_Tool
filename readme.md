This project package the required pyTorch library for JavaCpp pyTorch binding 1.10.2-1.5.7 to the debian file.

The javacpp PyTorch binding supports Cuda 11.3 in default, if want to support Cuda with other versions need to install
the required libtorch library with Cuda which want to use to the system library path,
also setting the "org.bytedeco.javacpp.pathsFirst" system property to "true".
    
### javacpp pytorch
    - version 
        1.10.2-1.5.7

### libtorch
    - version
        1.10.2 cu111
    - download link 
        https://download.pytorch.org/libtorch/cu111/libtorch-shared-with-deps-1.10.2%2Bcu111.zip
    - platform
        linux-x86_64
        
### Build
    mvn clean package

### Install
    dpkg -i 'deb file'
    **deb will install the lib to /usr/lib**