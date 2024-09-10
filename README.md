Download the weights 'best.pt' from the following link: https://drive.google.com/drive/folders/1VL3vKJF8Z77deqPKGr3ocCZ2DnBrKR0P?usp=drive_link

Paste 'best.pt' into the following location: yolov9/runs/train/exp3/weights/best.pt

Run this command:
```bash
cd yolov9
python test.py --imgsz 1280 --conf-thres 0.1 --device cpu --weights runs\\train\\exp3\\weights\\best.pt --source ..\\assets\\crash.jpeg
```
