# העלאת ה־PDF לריפו

הקובץ המקורי גדול יחסית, ולכן יש להעלות אותו כקובץ בינארי רגיל.

## יעד מדויק

```text
files/תחום אי וודאות.pdf
```

## דרך מומלצת ב־Termux

```bash
cd ~/storage/downloads
mkdir -p ~/i-vadaut-upload
cp "תחום אי וודאות.pdf" ~/i-vadaut-upload/
cd ~/i-vadaut-upload

git clone https://github.com/yanivmizrachiy/ahuzim.git
cd ahuzim
mkdir -p files
cp ~/i-vadaut-upload/"תחום אי וודאות.pdf" "files/תחום אי וודאות.pdf"

git add "files/תחום אי וודאות.pdf"
git commit -m "Add uncertainty domain PDF"
git push origin main
```

## שינוי שם הריפו ב־GitHub

Settings → Repository name → לשנות אל:

```text
i-vadaut
```

לאחר השינוי הכתובת תהיה:

```text
https://github.com/yanivmizrachiy/i-vadaut
```
