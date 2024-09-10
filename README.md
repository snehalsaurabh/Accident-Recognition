Download the weights 'best.pt' from the following link: https://drive.google.com/drive/folders/1VL3vKJF8Z77deqPKGr3ocCZ2DnBrKR0P?usp=drive_link

Paste 'best.pt' into the following location: yolov9/runs/train/exp3/weights/best.pt

## Way 1

Run this command:
```bash
cd yolov9
python findclass.py --imgsz 1280 --conf-thres 0.1 --device cpu --weights runs\\train\\exp3\\weights\\best.pt --source ..\\assets\\crash.jpeg
```

You can use any image. Crash.jpeg is just an example.

## Way 2

You can run automate.py to run the above command automatically. Just run the following command:
```bash
python automate.py
```
simply change the address of the image in the automate.py file.