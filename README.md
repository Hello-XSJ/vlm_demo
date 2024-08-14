# vlm_demo 视觉语言大模型

## 1. 功能介绍

`vlm_demo` 是在地平线 RDK 平台上在线调用大模型的通用型案例，用户可在 RDK 平台上也可在自己的 PC 机上在线体验 VLM 的强大功能。不论是在自己的 PC 机还是在 RDK 平台上，目前提供两种体验方式：
- 直接在终端输入文本与大模型进行自然对话；
- 或者是采用麦克风直接与大模型进行人机交互。

## 2. 物料清单

该系统可在以下平台上运行：
- RDK X3（4GB 内存）
- RDK Ultra
- PC 机（测试过 Ubuntu 18.04、20.04 和 22.04 的系统均无问题）
- USB 接口的麦克风（经测试有线耳机、蓝牙耳机均可）

## 3. 使用方法

### 3.1 准备工作

- 确认地平线 RDK X3 为 4GB 内存版本；
- 地平线 RDK X3 和 RDK Ultra 已烧录好地平线提供的 Ubuntu 20.04 系统镜像；
- 采用在线调用百度千帆和零一万物大模型。需要在对应官网上申请属于自己的 API Key，然后在 `vlm_demo` 中的 `API_KEY.py` 文件中替换成自己的 Key，方法参见官方文档说明：
  - [百度千帆](https://qianfan.cloud.baidu.com)
  - [零一万物](https://www.lingyiwanwu.com)

### 3.2 配置相关环境

以下是在 RDK 平台上配置的详细步骤，PC 机上的配置流程基本一致：

- 需要有 Python 3.9 环境。推荐使用 Miniforge，安装过程可参考 CSDN 中 Yabooo0 的文章：《Ubuntu 中安装 Miniforge》。使用 `conda` 创建一个新的环境用于配置大语言程序：
  ```bash
  conda create -n vlm python=3.9
 ---
