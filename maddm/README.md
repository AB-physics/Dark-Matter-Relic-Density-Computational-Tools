# Installing

```
conda create -n maddm python=3.8
```
```
conda activate maddm
```
```
conda deactivate
```
```
gfortran --version
make --version
cmake --version 
```

``` gfortran	10.5.0 ```
``` make	4.3	```
``` cmake	3.22.1 ```
```
sudo apt update
sudo apt install gfortran make cmake
```
```
wget https://launchpad.net/mg5amcnlo/3.0/3.6.x/+download/MG5_aMC_v2.9.24.tar.gz
tar xzf MG5_aMC_v2.9.24.tar.gz
cd MG5_aMC_v2_9_24
```
```
cd PLUGIN
git clone -b rc/3.3 --depth 1 --recurse-submodules --shallow-submodules https://github.com/maddmhep/maddm.git
```
```
cd MG5_aMC_v2_9_24/PLUGIN
mv maddm/maddm ../bin/maddm.py
cd ..
```
```
./bin/maddm.py
```
```
MadDM> install pythia8
```
```
MadDM> install PPPC4DMID
```
```
wget https://raw.githubusercontent.com/dimauromattia/darktools/refs/heads/main/maddm/DMsimp_s_spin1_MD.tar.gz
tar xf DMsimp_s_spin1_MD.tar.gz -C models
```
```
wget https://raw.githubusercontent.com/dimauromattia/darktools/refs/heads/main/maddm/ScalarHiggsPortal_NLO_UFO.tar.gz
tar xf ScalarHiggsPortal_NLO_UFO.tar.gz -C models
```
# Running
```
./bin/maddm.py
```
‍``` convert model models/DMsimp_s_spin1_MD ``` or ``` convert model /home/ahmad/Darkـmatter/MG5_aMC_v2_9_24/models/DMsimp_s_spin1_MD ``` or ``` set auto_convert_model T ```
```
MadDM> import model DMsimp_s_spin1_MD
```
```
MadDM> import model ScalarHiggsPortal_NLO_UFO
```
```
generate relic_density
```
```
generate direct_detection
```
```
generate indirect_detection
```
















