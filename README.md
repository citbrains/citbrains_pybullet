# citbrains_pybullet  
PyBullet simulator for SUSTAINA-OP  

SUSTAINA-OP is desinged by Masato Kubotera  
https://github.com/citbrains/SUSTAINA-OP

VIDEO  
[![IMAGE](http://img.youtube.com/vi/iXAvYs80RxA/0.jpg)](https://youtu.be/iXAvYs80RxA)

### Preparation of the development environment

Ubuntu2004  
```
sudo apt install python3-pip
pip install pybullet
pip install numpy
pip install control
git clone https://github.com/citbrains/GankenKun_pybullet
cd GankenKun_pybullet
python GankenKun.py
```

[Microsoft Windows](https://github.com/citbrains/GankenKun_pybullet/wiki/%E9%96%8B%E7%99%BA%E7%92%B0%E5%A2%83%E3%81%AE%E6%BA%96%E5%82%99) (in Japanese)

### main program

- walking_sample.py  
Walking control to the target position  

### library for GankenKun

walking/  

- kinematics.py  
Calculating the inverse kinematics based on the analytical solution  
(foot position -> joint angles)  

- foot_step_planner.py  
Calculating the footsteps from the goal position  

- preview_control.py  
Generating the trajectory of the center of mass from the footsteps based on the preview controller  

- walking.py  
Calculating the trajectory of the foot from the goal position  
