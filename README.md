Download the weights 'best.pt' from the following link: https://drive.google.com/drive/folders/1VL3vKJF8Z77deqPKGr3ocCZ2DnBrKR0P?usp=drive_link

Paste 'best.pt' into the following location: yolov9/runs/train/exp3/weights/best.pt

How to run the model.

1. Make a virtual environment.
```bash
python -m venv venv
```
2. Activate the virtual environment.
```bash
.\venv\Scripts\activate
```
3. Install the requirements. Come back to the main directory and run the following command.
```bash
pip install -r requirements.txt
```
4. Run the model using the given below commands.

## Way 1

Run this command:
```bash
cd yolov9
python findclass.py --imgsz 1280 --conf-thres 0.1 --device cpu --weights runs\\train\\exp3\\weights\\best.pt --source ..\\assets\\crash.jpeg
```

You can use any image. Crash.jpeg is just an example.

NOTE: If Way 2 and Way 3 are not working for you, in the code of custom_auto and automate.py, change the path of the python.exe file in the first line of the code to the path of the python.exe file in your virtual environment. It is hard coded to my virtual environment currently. 

## Way 2

You can run automate.py to run the above command automatically. Just run the following command:
```bash
python automate.py
```
simply change the address of the image in the automate.py file.

## Way 3

You can run the following command to run the above command automatically:
```bash
python automate.py "path_to_image"
```
you don't have to put the image path in the automate.py file. Just pass it as an argument. Don't forget to put the image in the assets folder. Use quotes if the path has spaces.
