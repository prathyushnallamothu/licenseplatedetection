# to train
python yolov5/train.py --img 640 --cfg yolov5s.yaml --hyp hyp.scratch-low.yaml --batch 16 --epochs 100 --data licence_plate_data.yaml --weights yolov5s.pt --workers 24 --name licence_detector 

# to detect 
 python yolov5/detect.py --source 0 --weights best.pt --conf 0.25 --name licence_detector