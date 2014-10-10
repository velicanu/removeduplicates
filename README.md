removeduplicates
================
Currently only works on Data where run+event number are a unique combination. 

Initial setup after cmsenv:
```bash
git clone git@github.com:CmsHI/HiForestAnalysis.git
g++ removeDuplicates.C $(root-config --cflags --libs) -std=c++11 -Werror -Wall -O2 -o removeDuplicates.exe
```
To run:
```bash
./removeDuplicates.exe <inputforest> <outputforest>
```
This will make a clone of the input forest with all the duplicate events stripped away. 
