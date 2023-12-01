### Building image using Apple Silicon (M1/M2) ARM64
1. Build 2.10.1 ckan-base image
```
cd ckan-2.10/base
make build
```
_Resulting local images:_ **ckan/ckan-base:2.10, ckan/ckan-base:2.10.1**

2. Build 2.10.1 ckan-dev image  (will use local image from step a)
```
cd ../dev
make build
```
_Resulting local images:_ **ckan/ckan-dev:2.10, ckan/ckan-dev:2.10.1**

3. Build datapusher image
```
cd ../../datapusher 
make build
```
_Resulting local image:_ **ckan/ckan-base-datapusher:0.0.20**