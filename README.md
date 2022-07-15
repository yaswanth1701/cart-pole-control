# Cart-Pole Control
![screenshot](https://user-images.githubusercontent.com/92177410/177828130-e6b4d092-40fd-439d-bd4b-a5d0363f0c1d.png)
## PID Control of Inverted Pendulum
Here PID control was used to stabilize the inverted pendulum in upright position. It was observed that a large amount of force is applied initially. From the graphs it can be seen that the value of x is increasing ie the cart keeps on moving towards right.


<img src="https://user-images.githubusercontent.com/92177410/178713705-9a805e46-c189-4005-baec-e57a7cd0bf27.png" width="300" height="200">
<img src="https://user-images.githubusercontent.com/92177410/178713497-03787c9c-819d-444a-8ca2-238d02c8b1e4.png" width="300" height="200">


## LQR Control of Inverted Pendulum
Here we build an LQR controller to stabilize the pendulum in upright position. We tunned the Q (penalty on states) and R (penalty on actuators) matrix to obtain the desired results. Below graphs shows variation of theta, force, postion(x) with time. In animation we can see pendulum stabilize in upright postion at desired (x=5).

<img src="https://user-images.githubusercontent.com/92177410/179186956-ce539d08-86b6-408a-8a58-21f193789ac6.png" width="300" height="300">


## Inverted Pendulum(LQR + Energy Control)
This is a hybrid approach to Inverted pendulum. Here we use Energy Control along with LQR to make the pendulum stand at upright position.
What we observed is LQR is unable to take the pendulum directly to the upright position in a efficient manner and it also gives absurd results when did so.
So In hybrid model the changes done are intially directly the corresponding energy at upright position is given to the pendulum and as it reaches close to vertical force is applied through LQR model. In this way we get better graphs and there is no need to apply caps on any of the quantity.

![]()
<img src="https://i.imgur.com/8nesENw.gif" width="300" height="200">

<img src="https://user-images.githubusercontent.com/92177410/179187940-f3a1fc06-a91c-4f5b-a260-ccf3bb1ea6ac.png" width="300" height="200">
<img src="https://user-images.githubusercontent.com/92177410/179187969-4de55f90-0935-4d39-8954-747ed7fcace1.png" width="300" height="200">
<img src="https://user-images.githubusercontent.com/92177410/179187983-9748b4ef-f767-4687-b646-1bda731134f1.png" width="300" height="200">
