#  android အသုံးပြုပြီး service accounts လုပ်နည်း

- [x] အရင်ဆုံး Termux ကို မိမိဖုန်းထဲ install လုပ်ပါ
[Termux Download Link](https://drive.google.com/uc?export=download&id=19VycS90NijIR1u_KYTumRJDu4c2xKK7P)
install လုပ်ပီးရင် Termux ကိုဖွင်လိုက်ပါ
​အောက်က CMD ​တွေ ရိုက်ထည့်ပါ
```
termux-setup-storage
```
```
pkg update
```
```
pkg upgrade 
```
```
pkg install git
```
```
pkg install python
```
```
pip install --upgrade pip
```
```
mkdir /sdcard/MyTermux/ -p
```
```
cd /sdcard/MyTermux
```
```
git clone https://github.com/phoethar1/service-accounts
```
```
cd /sdcard/MyTermux/service-accounts
```
```
pip3 install -r requirements.txt
```
credentials.json file ကို [Google Console](https://console.cloud.google.com/?pli=1)မှာပြုလုပ်ပါ

```
python3 gen_sa_accounts.py --quick-setup -1
```
python3 gen_sa_accounts.py  --download-keys Project ID
Project ID​နေရာမှာ မိမိ Project IDထည့်

```
python generate_drive_token.py
```
```
cd accounts
```
```
python3 emails.py
```