# FCC-softwares
## Installing FCCAnalysis
To install FCCAnalysis, first we need to source 
```
source /cvmfs/sw.hsf.org/key4hep/releases/2024-10-03/x86_64-almalinux9-gcc14.2.0-opt/key4hep-stack/2024-10-08-k6xtr3/setup.sh
```
If ```2024-10-03``` is not working change it to the latest.
```
source /cvmfs/fcc.cern.ch/sw/latest/setup.sh
```
```
source /cvmfs/sw.hsf.org/key4hep/setup.sh
```
Get clone the ```FCCAnalysis.git``` from the github
````
git clone main https://github.com/HEP-FCC/FCCAnalyses.git
cd FCCAnalysis
```
```
source setup.sh
```
Create build and install directories and move to build directory.
```
mkdir build install && cd build
```
```
cmake .. -DCMAKE_INSTALL_PREFIX=../install
```
```
make install -j $(nproc)
```
