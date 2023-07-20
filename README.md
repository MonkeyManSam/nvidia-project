# nvidia-project
Age Detector is a machine learning project that uses NVIDIA's Jetson Nano bot and a Kaggle dataset to estimate the age of a person based on an image. The machine learning model is trained using the ImageNet and ResNet-18 machine learning programs.

Installation
1. Connect the nano using putty app on serial to get the ip address for later
2. Log in to the terminal using the username: nvidia: and password: nvidia
3. Clone the repository.
4. Install jetson_Inference
5. Change directory to Jetson_Inference and run this command: ./docker/run.sh
6. While in the docker navigate to python/training/classification/models/age_guess
7. Run the command "imagenet.py --model=resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt /dev/video0"
8. Show images to the camera and it will predict the age
