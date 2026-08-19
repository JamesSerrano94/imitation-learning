

Just run the Google Colab file and follow the instructions.

**WARNING**

Note, because mujoco API has updated, code no longer works. However the video is a demonstration of what the AI is trained to do. However this is an image of the robot working in action.

**What is this**

The short answer is this is a demonstration of imitation learning algorithm. You give a robot successful demonstrations of whatever objective it needs to complete and then it uses Machine Learning methods in order to reverse intuit the user's intentions.

This is a demonstration of how to teach a robotic arm to preform a variety of tasks using a Generative Adversarial Network. This project uses the Mujoco API, which provides the physics simulation of the arm. The demonstrations are in h5py format provided by the link in the google doc at the beginning of the Juypiter notbeook. What this project does is it takes successful demonstrations of various tasks being done, uses a GAN to output a neural network which provides a policy which can guide the robot to complete the task.

**Results**

There were multiple tasks: Picking up a brick, placing a brick on top of a larger brick, putting trash in a trash bin, putting trash in a trash bin and then closing the trash bin but also ignoring non-trash items. Being able to pick up a brick works with 100% efficiency but more complex tasks work 8-13% of the time. I believe this can be overcome with more hyperparameter tuning, such as increasing the number of epochs or adjusting the alpha and gamma rates, and seeing how changing these values affects both the effectiveness of the Generative and Adversarial Neural Networks.

**Challenges, limitations and future plans**

Through this project I analyzed several different immitation learning architecture, and settled on INFOGAIL. The reason is that the GAN architecture was more versatile than something like TRajectory-EXtrapolation or using a Pointcloud Probability Curve. The architecture could be applied to many different tasks but often failed when the task required increasing complexity.

<img width="487" height="444" alt="image" src="https://github.com/user-attachments/assets/e3c2ff7c-8724-4444-abe2-204090bc6193" />


[![DEMO](https://i.imgur.com/2Dbufyf.mp4)](https://i.imgur.com/2Dbufyf.mp4)
