# Cart-Pole Control
![screenshot](https://user-images.githubusercontent.com/92177410/177828130-e6b4d092-40fd-439d-bd4b-a5d0363f0c1d.png)
## PID Control of Inverted Pendulum
Here PID control was used to stabilize the inverted pendulum in upright position. It was observed that a large amount of force is applied initially. From the graphs it can be seen that the value of x is increasing ie the cart keeps on moving towards right.
![image](https://user-images.githubusercontent.com/92177410/178713705-9a805e46-c189-4005-baec-e57a7cd0bf27.png)

![image](https://user-images.githubusercontent.com/92177410/178713497-03787c9c-819d-444a-8ca2-238d02c8b1e4.png)



## LQR Control of Inverted Pendulum
Here we build an LQR controller to stabilize the pendulum in upright position. We tunned the Q (penalty on states) and R (penalty on actuators) matrix to obtain the desired results. Below graphs shows variation of theta, force, postion(x) with time. In animation we can see pendulum stabilize in upright postion at desired (x=5).



![ngM1cxZ](https://user-images.githubusercontent.com/92177410/178701255-7f320f35-8f50-4265-8cbc-6deea8b730c6.png)


## Inverted Pendulum(LQR + Energy Control)
This is a hybrid approach to Inverted pendulum. Here we use Energy Control along with LQR to make the pendulum stand at upright position.
What we observed is LQR is unable to take the pendulum directly to the upright position in a efficient manner and it also gives absurd results when did so.
So In hybrid model the changes done are intially directly the corresponding energy at upright position is given to the pendulum and as it reaches close to vertical force is applied through LQR model. In this way we get better graphs and there is no need to apply caps on any of the quantity.

![image](https://user-images.githubusercontent.com/92177410/178711296-93a8b406-2732-44f6-9c2c-6af4570132ec.png)


![image](https://user-images.githubusercontent.com/92177410/178711169-e35ea2b0-3b38-408f-8589-79dbc3d75590.png)

![image](https://user-images.githubusercontent.com/92177410/178711376-b51847d6-82fd-4093-80c8-cb86e5ca409e.png)

![image](https://user-images.githubusercontent.com/92177410/178711406-ae802936-c2cb-4944-8804-4c6ffab2fdb8.png)


