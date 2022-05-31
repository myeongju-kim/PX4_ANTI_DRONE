<div align="center">
  <h1 align="center">ANTI-DRONE DEVELOPMENT</h1>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#quick-start-examples">Quick Start Examples</a></li>
      </ul>
    </li>
    <li><a href="#execution-flow">Execution Flow</a></li>
    <li><a href="#contribution">Contribution</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This project developed anti-drone utilizing px4 autopilot open source.


#### What is an anti-drone?
>With the development of drone technology, drones are rapidly emerging as new social safety threats in various fields such as crime and terrorism.
As a result, 'anti-drones' emerged as a concept of a kind of air defense platform to respond to drone threats.

#### What is PX4 Autopilot?
> PX4 autopilot is an open-source autopilot system oriented toward inexpensive autonomous aircraft.<br>
Low cost and availability enable hobbyist use in small remotely piloted aircraft. The project started in 2009 and is being further developed and used at Computer Vision and Geometry Lab of ETH Zurich (Swiss Federal Institute of Technology) and supported by the Autonomous Systems Lab and the Automatic Control Laboratory. Several vendors are currently producing PX4 autopilots and accessories.
<br>✔ We referred here https://docs.px4.io/master/en/


### Built With

List frameworks/libraries in my project.

* [PX4](https://github.com/PX4/PX4-Autopilot)
* [ROS](https://docs.ros.org/en/foxy/index.html)
* [QGC](http://qgroundcontrol.com/)
* [SITL](https://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html)
* [YOLOv5](https://github.com/ultralytics/yolov5)



## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites
* Recommended in ubuntu environment and versions >= 18.04.
* Install ROS ([we used ros2 foxy version](https://docs.ros.org/en/foxy/index.html))
* Install PX4 
```
git clone https://github.com/PX4/PX4-Autopilot.git
```
### Quick Start Examples

   ```
    git clone https://github.com/myeongju-kim/PX4_ANTI_DRONE.git
    cd PX4_ANTI_DRONE
   ```
* If you want to use gps_spoofing
```
git clone https://github.com/PX4/PX4-Autopilot.git
cp -r PX4_ANTI_DRONE/execution PX4-Autopilot/src
```
* If you want to use drone identification<br>
✔ Since the drone image file is not provided, if you want to use it, you need to download a drone large-capacity image from Kaggle.<br>
✔ Python >= 3.7.0 environment, including PyTorch >= 1.7.
```
git clone https://github.com/ultralytics/yolov5  # clone
cd yolov5
pip install -r requirements.txt  # install
```

## Execution Flow
![image](https://user-images.githubusercontent.com/83527620/172048445-dee522cc-a750-419c-a02f-0693196bea12.png)
* Use LIDAR sensor (you can find it feature/detection_RF)
* Use QGC and GAZEBO to take off the drone
* Use YOLOv5 (you can find it feature/detection_yolov5)
* Use GPS spoofing (you can find it feature/gps_spoofing)


## Contribution
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch 
3. Commit your Changes 
4. Push to the Branch
5. Open a Pull Request

## License
[PX4 Flight Stack](https://github.com/PX4/PX4-Autopilot) — BSD<br>
[PX4 Middleware](https://github.com/PX4/PX4-Autopilot) — BSD<br>
[Pixhawk Hardware](https://github.com/pixhawk/Hardware) — CC-BY-SA 3.0<br>
[PX4 User Guide](https://github.com/PX4/PX4-user_guide) — CC BY 4.0 (opens new window)
## Contact

mjoo1106@khu.ac.kr<br>
sksm2020@khu.ac.kr
