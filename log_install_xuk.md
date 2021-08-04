# Logs on installation process by Ke Xu

```
logs on the installation process of sokrg package
initiated by Ke Xu (kxu4143@sdsu.edu)
first commit on 07/22/2021
```

## 1/ packages needed for R codes:
  - conda: install miniconda (Python3.9 MacOs package):
```
bash Miniconda3-latest-MacOSX-x86_64.sh
```
  - requirements based on yml file in the sokrg package:
```
conda env create -f requirements.yml
conda activate sokrg
```
  - R scripts: downloaded R-4.1.0.pkg for MacOs and installed directly
  - gstat package (v2.0_7): conda install -c conda-forge r-gstat
  - sp package (v1.3_1): conda install -c r r-sp

## 2/ environment & library settings
  - error encountered: dyld: Library not loaded: @rpath/libreadline.6.2.dylib.  
    [solved by]
```
conda update -c rdonnellyr -c main --all
```
