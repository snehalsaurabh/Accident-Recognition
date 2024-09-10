Paste 'best.pt' into the following location: yolov9/runs/train/exp3/weights/best.pt

Run this command:
```bash
cd yolov9
python test.py --imgsz 1280 --conf-thres 0.1 --device cpu --weights runs\\train\\exp3\\weights\\best.pt --source ..\\assets\\crash.jpeg
```
