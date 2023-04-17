# Super-Mario-Agent-PPO-Python
## :bangbang: C. Unexpected problems and solutions:
1.	When you run pip to install nes-py, you might encounter the error python bdist_wheel did not run successfully <br />
    :point_right: **_Solution_**: you need install MSVC - v140 VS2015 C++ Build Tools (v14.00) and Windows 10 SDK 10.0.20348.0, then add a new value to the Environment Variable PATH: C:\Program Files (x86)\Windows Kits\10\bin\x64. After that Copy the file rc.exe & rcdll.dll from C:\Program Files (x86)\Windows Kits\10\bin\10.0.20348.0\x64 to C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\bin. Rerun it again.

2.	When you run GrayScaleObservation you might encounter the problem with not finding module CV2. Note that CV2 is part of the OpenCV library, which is not installed by default with Anaconda and it’s important to run module gym.wrappers.gray_scale_observation <br />
    :point_right: **_Solution 1_**: !pip install opencv-python <br />
    :point_right: **_Solution 2_**: !pip install stable-baselines3[extra] (it include opencv-python)<br />
