

Just run the Google Colab file and follow the instructions.

**WARNING**

Note, because mujoco API has updated, code no longer works. However the video is a demonstration of what the AI is trained to do. However this is an image of the robot working in action

**What is this**

This is a demonstration of how to teach a robotic arm to preform a variety of tasks using a Generative Adversarial Network. The framework is Mujoco, which provides the simulation of the arm. The demonstrations are in h5py format provided by the link in the google doc. The model then takes these demonstrations and outputs a neural network which uses a GAN to provide a policy which can guide the robot in it's task.

**Results**

Depends on the task. Being able to pick up a brick works with 100% efficiency but more complex tasks like folding laundry work 8-13% of the time. I believe this can be overcome with more hyperparameter tuning, such as increasing the number of epochs or fooling around with alpha and gamma rates, and seeing how changing these values affects both the effectiveness of the Generative and Adversarial Neural Networks.

**Challenges, limitations and future plans**

Through this project I analyzed several different immitation learning architecture, and settled on INFOGAIL. The reason is that the GAN architecture was more versatile than something like TRajectory EXtrapolation or using a pointcloud. The architecture could be applied to many different tasks but often

<img width="487" height="444" alt="image" src="https://github.com/user-attachments/assets/e3c2ff7c-8724-4444-abe2-204090bc6193" />


[![DEMO](https://i.imgur.com/2Dbufyf.mp4)](https://i.imgur.com/2Dbufyf.mp4)
