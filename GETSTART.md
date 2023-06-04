
### [Data-Preparation](https://mmdetection3d.readthedocs.io/en/latest/user_guides/dataset_prepare.html)

* if `No module named 'tools.dataset_converters'`:
```
export PYTHONPATH=.
```


### Training

[MVX-Net](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/mvxnet):
```
python tools/train.py configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py
```
[PV-RCNN](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/pv_rcnn):
```
python tools/train.py configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py
```
[3D-SSD](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/3dssd):
```
python tools/train.py configs/3dssd/3dssd_4xb4_kitti-3d-car.py
```
[SA-SSD](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/sassd):
```
python tools/train.py configs/sassd/sassd_8xb6-80e_kitti-3d-3class.py
```


### Testing and Inference

[MVX-Net](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/mvxnet):
```
python tools/test.py configs/mvxnet/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class.py work_dirs/mvxnet_fpn_dv_second_secfpn_8xb2-80e_kitti-3d-3class/epoch_40.pth
```
[PV-RCNN](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/pv_rcnn):
```
python tools/test.py configs/pv_rcnn/pv_rcnn_8xb2-80e_kitti-3d-3class.py work_dirs/pv_rcnn_8xb2-80e_kitti-3d-3class/epoch_40.pth
```
[3D-SSD](https://github.com/open-mmlab/mmdetection3d/tree/main/configs/3dssd):
```
python tools/test.py configs/3dssd/3dssd_4xb4_kitti-3d-car.py work_dirs/3dssd_4xb4_kitti-3d-car/epoch_80.pth
```
