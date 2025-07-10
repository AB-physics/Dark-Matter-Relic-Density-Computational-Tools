# Installing
ساخت محیط conda با پایتون:
```
conda create -n maddm python=3.8
```
```
conda activate maddm
```
```
conda deactivate
```
نصب پیش‌نیازهای سیستمی:
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
دانلود و استخراج MadGraph v2.9.24:
```
wget https://launchpad.net/mg5amcnlo/3.0/3.6.x/+download/MG5_aMC_v2.9.24.tar.gz
tar xzf MG5_aMC_v2.9.24.tar.gz
cd MG5_aMC_v2_9_24
```
وارد پوشه PLUGIN شده و MadDM را از شاخه rc/3.3 کلون کنید:
```
cd PLUGIN
git clone -b rc/3.3 --depth 1 --recurse-submodules --shallow-submodules https://github.com/maddmhep/maddm.git
```
```
cd MG5_aMC_v2_9_24/PLUGIN
mv maddm/maddm ../bin/maddm.py
cd ..
```
اجرای MadDM:
```
./bin/maddm.py
```
نصب ابزارهای مورد نیاز داخل محیط MadDM:
```
MadDM> install pythia8
```
```
MadDM> install PPPC4DMID
```
دانلود و استخراج دو مدل DM:
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
تبدیل خودکار مدل‌ها (برای Python 3)
داخل کنسول MadDM:
‍``` convert model models/DMsimp_s_spin1_MD ``` or ``` convert model /home/ahmad/Darkـmatter/MG5_aMC_v2_9_24/models/DMsimp_s_spin1_MD ``` or ``` set auto_convert_model T ```
```
MadDM> import model DMsimp_s_spin1_MD
```
```
MadDM> import model ScalarHiggsPortal_NLO_UFO
```
بعد از import کردن هر مدل، می‌توانید دستورات محاسباتی را اجرا کنید:
این دستورات به ترتیب چگالی بقای ماده تاریک، آشکارسازی مستقیم (بر­هم‌کنش با نوکلئون یا الکترون) و آشکارسازی غیرمستقیم را محاسبه و نتایج را تولید می‌کنند.
```
generate relic_density
```
```
generate direct_detection
```
```
generate indirect_detection
```
```
MadDM> launch
```















