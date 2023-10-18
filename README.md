# Railroad-dataset
This repository shares some simultaneous localization and mapping (SLAM) datasets and detection datasets for railroad application. Note that this sahring is a continuous and long-during process due to complicated legal issues and safety regulations on the railroad. </br>
In the first stage, we decide to realease some LiDAR, visual, IMU sequence for freight-traffic railways. The ground truth cannot be provided due to safety regulations. </br>
The single LiDAR sequence: </br>
1. Velodyne VLP16 LiDAR, provided in pcap format, gathered on a maintenance vehicle. </br>
![image](https://user-images.githubusercontent.com/40022787/161363298-92677049-5d4b-49ef-b0a6-4a40088c9270.png)</br>
links:</br>
2. Ouster OS1-64 LiDAR, provided in rosbag format, gathered on a UGV on a newly constructed high-speed railway. </br>
![image](https://user-images.githubusercontent.com/40022787/161363284-d5d26c89-0587-4c19-89ef-eebe5c2ac4c8.png)</br>
links:</br>
Topics
```C++
/ouster_points          Ouster point clouds 
/imu/data               IMU measurements provided by MTI-680G
```
3.  Livox LiDAR, provided in rosbag format, gathered on several maintenance vehicles, inlcuding single lidar, multiple lidar datasets. </br>
single LiDAR: </br>
![image](https://user-images.githubusercontent.com/40022787/161363343-01a6a8de-88d3-410c-ab33-332e1142d5ee.png)</br>
links: 链接：https://pan.baidu.com/s/1wjItY9bns6SUwzAvF-mIxA?pwd=7mtr 提取码：7mtr </br>
Topics:
```C++
/livox/lidar            Livox lidar in custom_msg format, note that both livox horizon and avia is included 
/imu/data               IMU measurements provided by MTI-680G
```
4. mutiple LiDAR:</br>
![0c70d5fc6befd873355f9f51d787adb](https://user-images.githubusercontent.com/40022787/161363480-58f26153-53eb-4040-addb-5263c42966ba.jpg)</br>
links:链接：https://pan.baidu.com/s/1ndYHlKrkQ2aWSdJtsfAmBg?pwd=cp6e 提取码：cp6e  </br>
Although up to 7 or 8 LiDARs are included in our system, we only provide the front two LiDARs information here due to safety regulations. </br>
```C++
/livox/lidar_1xxxx            The downview lidar 
/livox/lidar_3xxxx            The upview lidar 
/imu/data                     IMU measurements provided by MTI-680G
```
