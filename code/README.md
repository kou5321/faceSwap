# FaceSwap
Swap face between two photos for Python 3 with OpenCV and dlib.

## Intro to dlib
It‘s a landmark’s facial detector with pre-trained models, 
the dlib is used to estimate the location of 68 coordinates (x, y) 
that map the facial points on a person’s face.
[Facial mapping (landmarks) with Dlib + python](https://towardsdatascience.com/facial-mapping-landmarks-with-dlib-python-160abcf7d672)
## Get Started
```sh
python main.py --src imgs/test6.jpg --dst imgs/test7.jpg --out results/output6_7.jpg --correct_color
```

[//]: # (| Source | Destination | Result |)

[//]: # (| --- | --- | --- |)

[//]: # (|![]&#40;imgs/test6.jpg&#41; | ![]&#40;imgs/test7.jpg&#41; | ![]&#40;results/output6_7.jpg&#41; |)

```sh
python main.py --src imgs/test6.jpg --dst imgs/test7.jpg --out results/output6_7_2d.jpg --correct_color --warp_2d
```

| Source | Destination | Result |
| --- | --- | --- |
|![](imgs/test6.jpg) | ![](imgs/test7.jpg) | ![](results/output6_7_2d.jpg) |


### Swap Your Face
```sh
python main.py ...
```
Note: Run **python main.py -h** for more details.

### Real-time camera
```sh
python main_video.py --src_img imgs/test7.jpg --show --correct_color --save_path {*.avi}
```

### Video
```sh
python main_video.py --src_img imgs/test7.jpg --video_path {video_path} --show --correct_color --save_path {*.avi}
```

## More Results
| From | To |
| --- | --- |
| ![](imgs/test4.jpg) | ![](results/output6_4.jpg) |
| ![](imgs/test3.jpg) | ![](results/output6_3.jpg) |
| ![](imgs/test2.jpg) | ![](results/output6_2_2d.jpg) |
| ![](imgs/test1.jpg) | ![](results/output6_1.jpg) |
| ![](imgs/test4.jpg) | ![](results/output7_4.jpg) |
