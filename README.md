# Human Pose Estimation

This repository provides implementation for ***Human Pose Estimation*** that predicts the location of various human keypoints (joints and landmarks) such as elbows, knees, neck, shoulder, hips, chest etc.

## Requirements
- OpenCV
- OpenPose

## Usage
- To download the pre-Trained models, run `sh get_model.sh` command.
- To run pre-Trained model, trained on ***MPII Human Pose*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/mpi/pose_deploy_linevec_faster_4_stages.prototxt --model human_pose_proto/mpi/pose_iter_160000.caffemodel --dataset MPI`.
- To run pre-Trained model, trained on ***COCO*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/coco/deploy_coco.prototxt --model human_pose_proto/coco/pose_iter_440000.caffemodel --dataset COCO`.
- To run pre-Trained model, trained on ***Body_25*** dataset, on any image, run the following command:-
`python3 human_pose_estimation.py --input <Image Name> --proto human_pose_proto/body_25/body_25_deploy.prototxt --model human_pose_proto/body_25/pose_iter_584000.caffemodel`.

## Results

Following are a few ***human poses*** predicted by the model:-
| Test Image        | Generated Keypoint Skeleton           |
| ------------------- |:----------------------------:|
| <img src="https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample.jpg" height="495"> | <img src="https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample_result.webp" height="495"> |
| <img src="https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample2.jpg" width="320"> | <img src="https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample2_result.webp" width="320"> |
<!-- | <img src="https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/7NNg0_n-bS8_21_30.gif" width="320"> | a man is performing on a stage | -->
<!-- | ![alt text](https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample.jpg) | ![alt text](https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample_result.webp) |
| ![alt text](https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample2.jpg) | <img src="https://github.com/fork123aniket/Human-Pose-Estimation/blob/main/images/sample2_result.webp" height="395"> |
| <img src="https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/7NNg0_n-bS8_21_30.gif" width="320"> | a man is performing on a stage | -->

