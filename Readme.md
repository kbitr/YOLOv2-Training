# Read-to-run YOLOv2 Training


```bash
git clone https://github.com/kbitr/YOLOv2-Training
cd YOLOv2-Training
curl -O https://pjreddie.com/media/files/darknet19_448.conv.23
git clone https://github.com/pjreddie/darknet
cd darknet
make

./darknet detector train ../stop.data ../stop.cfg ../darknet19_448.conv.23
```

Thats's it! You should edit the Makefile to GPU=1, CUDNN=1, OPENMP=1  or similar for faster training before executing _make_.

###### Disclaimer: Yes, I am too lazy to set darknet as a submodule.