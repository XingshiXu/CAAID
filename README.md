# CAAID ![](https://img.shields.io/badge/contributor-XingshiXu-brightgreen.svg)

Cattle Information Intelligent Acquisition Device

在精准养殖（PLF）的框架下，设计牛只信息智能采集装置具有重要意义。PLF注重数据驱动的决策和精准管理，而牛只各项信息的准确性、实时性和全面性对于养殖效率和健康管理至关重要。为此，该repo持续更新我们设计的背负式牛只信息智能采集装置(Cattle Information Intelligent Acquisition Device, CAAID)。我们认为它有以下几方面的优势：
- **数据精准度和实时性**：智能采集装置可以在牛只的日常活动中实时采集数据，避免了手工记录可能带来的错误和延迟，确保了数据的精准性和实时性。
- **综合信息采集**：装置可以同时采集多个方面的信息，如身份信息、体尺、体重、体况、清洁度、发情状况以及用药情况等，使得养殖管理者能够全面了解每头牛的状况，为精准决策提供数据支持。
- **智能分析与预警**：采集装置可以通过内置的智能算法对数据进行分析，发现异常情况并提供预警，使养殖管理者能够及时采取措施，防止疾病传播或其他问题的发生。
- **劳动力节约与效率提升**：相比于传统的手工记录或测量，智能采集装置可以相对自动的完成数据采集和处理，节约了人力资源，并提高了数据管理的效率和准确性。
- **远程监控与管理**：采集的数据可以通过网络传输至远程服务器，允许养殖场管理者随时随地监控牛只的情况，及时调整养殖策略和管理措施，提高养殖效率和利润。


如图1a所示，该设备由Nvidia Jetson AGX Orin、摄像头(ZED 2i)、电源、显示屏以及其他多个辅助功能模块组成。如图1b，使用者可以轻松的通过如图2c所示的用户交互界面操作系统设备终端实现牛只各类信息的手动输入或自动测量以及进行信息查看。所有的记录信息能够通过MQTT穿透上传到服务器的数据库中。这些数据将有助于农民、兽医做出更加准确的决策。
![示例图片1](https://github.com/XingshiXu/CAAID/blob/main/Example%20image1.jpg)


======
目前已实现的功能：Y:yes N:no W:waiting to be extended  N\A: not applicable
| 功能       | 手动输入 | 自动识别 | 备注  |
|:----------:|:-------:|:--------:|:-----:|
| 牛只身份   |    Y    |    Y     |  N\A  |
| 牛只计数   |    Y    |    Y     |  N\A  |
| 清洁度评分 |    Y    |    N     |  N\A  |
| 体尺测量   |    Y    |    N     |  N\A  |
| 体重预估   |    Y    |    N     |  N\A  |
| 体况记录   |    Y    |    N     |  N\A  |
| 用药记录   |    Y    |   N\A   |  N\A  |
| 发情监测   |   N\A   |    Y    | [Link](https://github.com/XingshiXu/CAAID/blob/main/estrus.md) |
| 跛行检测   |    W    |    W     |  N\A  |
| 行为分析   |   N\A   |   N\A    |  N\A  |

======

主界面

![主界面](https://github.com/XingshiXu/CAAID/blob/main/mainGUI.gif)

---------------
个体识别界面

![个体识别界面](https://github.com/XingshiXu/CAAID/blob/main/IDcow1.gif)

-------------
体尺测量界面
![体尺界面]([https://github.com/XingshiXu/

---------





目前我们的装置还处于开发阶段，一些功能并没有完成部署。我们将持续的更新这一repo，以展示这一产品的最新功能。同时我们的最新研究将展示在https://github.com/XingshiXu/HingsWorks


