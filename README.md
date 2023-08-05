# MakeItTalk: Speaker-Aware Talking-Head Animation

This repo contains some experiments I did to explore cartoon character animation. It's forked from [this](https://github.com/yzhou359/MakeItTalk) repo.


If we focus on full-body animation, we can use [Thin Plate Spline Motion Model](https://github.com/yoyo-nb/Thin-Plate-Spline-Motion-Model), which needs 10+ short video clips for training. Existent models don’t work since they are trained on real human videos. 
This repo mainly focuses on cartoon face talking head animation, which is based on 2D image warping and LSTM. It depends only on a single image with built-in non-human landmark detector. There's another newer method called [SadTalker](https://github.com/OpenTalker/SadTalker) which is based on 3D face model and Stable Diffusion. It just needs a single image for training. However, it can’t detect face landmarks for non-human characters. 


Below are some test results:
## landmark detection
![img](/examples_bunny/angelbaby_anno.png)
## close mouth approximation
![img](/examples_bunny/angelbaby_face_close_mouth.png)
## delauney results
![img](/examples_bunny/angelbaby_delauney_1.png)
## final result
[![Watch the video](/examples_bunny/angelbaby.png)](/examples_bunny/final_output.mp4)

