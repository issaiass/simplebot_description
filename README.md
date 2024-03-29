# simplebot_description


<details open>
<summary> <b>Brief Review<b></summary>

simplebot_description is in charge to launch in rviz and gazebo the fusion 360 urdf exported model.

Now, with Google Cartographer, we can navigate and build the map of the room in this case, 2D.

### <b>Simplebot Google Cartographer</b>
<p align="center">
<img src = "doc/gif/simplebot_cartographer.gif?raw=true" center=true width="85%"/>
</p>


### <b>Simplebot Teleoperation</b>
<p align="center">
<img src = "doc/gif/simplebot_gazebo_ros2.gif?raw=true" center=true width="85%"/>
</p>


### <b>Simplebot Gazebo</b>
<p align="center">
<img src = "doc/imgs/simplebot_gazebo_view.PNG?raw=true" center=true width="85%"/>
</p>

### <b>Simplebot rviz2</b>
<p align="center">
<img src = "doc/imgs/simplebot_rviz2_view.PNG?raw=true" center=true width="85%"/>
</p>

### <b>Simplebot rqt_graph</b>
<p align="center">
<img src = "doc/imgs/simplebot_rqt_graph_view.PNG?raw=true" center=true width="85%"/>
</p>


</details>

<details open>
<summary> <b>Using the Package<b></summary>

- Follow the next steps to replicate the outcome
- On the first terminal
~~~
    cd ~/ros2_ws/src
    git clone https://github.com/issaiass/simplebot_description.git
    git clone https://github.com/issaiass/simplebot_slam.git    
    cd ~/ros2_ws
    colcon build --packages-select simplebot_description simplebot_slam
    ros2 launch simplebot_description display.launch.py
~~~

- On the second terminal
~~~
    ros2 launch simplebot_slam cartographer.launch.py
~~~

- If not selected, select the odom frame

- On the third terminal
~~~
    ros2 run teleop_twist_keyboard teleop_twist_keyboard
~~~

- Press the keys suggested to move the robot
- put an object in front of the robot
- view the rviz2 window, you will find the lidar points in red.

<details open>
<summary> <b>Results<b></summary>

Last video update - Simplebot Cartographer

[<img src= "https://img.youtube.com/vi/yC8pVZDEJEQ/0.jpg" />](https://youtu.be/yC8pVZDEJEQ)

[Simplebot Teleoperation](https://youtu.be/-lZ4t5rnFIk)

<p align="center"> </p>
</details>



<details open>
<summary> <b>Issues<b></summary>

- No issues encountered right now, but probably the caster_joint is not at the position desired, is not a problem.
- If the robot slips over time you need to change mu1 and mu2 over the .gazebo file in urdf folder

</details>

<details open>
<summary> <b>Future Work<b></summary>

- No further work.

</details>

<details open>
<summary> <b>Contributing<b></summary>

Your contributions are always welcome! Please feel free to fork and modify the content but remember to finally do a pull request.

</details>

<details open>
<summary> :iphone: <b>Having Problems?<b></summary>

<p align = "center">

[<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/riawa)
[<img src="https://img.shields.io/badge/telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/>](https://t.me/issaiass)
[<img src="https://img.shields.io/badge/instagram-%23E4405F.svg?&style=for-the-badge&logo=instagram&logoColor=white">](https://www.instagram.com/daqsyspty/)
[<img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" />](https://twitter.com/daqsyspty) 
[<img src ="https://img.shields.io/badge/facebook-%233b5998.svg?&style=for-the-badge&logo=facebook&logoColor=white%22">](https://www.facebook.com/daqsyspty)
[<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/riawe)
[<img src="https://img.shields.io/badge/tiktok-%23000000.svg?&style=for-the-badge&logo=tiktok&logoColor=white" />](https://www.linkedin.com/in/riawe)
[<img src="https://img.shields.io/badge/whatsapp-%23075e54.svg?&style=for-the-badge&logo=whatsapp&logoColor=white" />](https://wa.me/50766168542?text=Hello%20Rangel)
[<img src="https://img.shields.io/badge/hotmail-%23ffbb00.svg?&style=for-the-badge&logo=hotmail&logoColor=white" />](mailto:issaiass@hotmail.com)
[<img src="https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" />](mailto:riawalles@gmail.com)

</p

</details>

<details open>
<summary> <b>License<b></summary>
<p align = "center">
<img src= "https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-sa.svg" />
</p>
</details>
