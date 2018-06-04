# cat_vs_dog
猫狗识别问题


1. 基于python3.6使用的库有：
numpy pandas sklearn matplotlib seaborn h5py  jupyter pillow tensorflow-gpu keras tqdm  cv2 graphviz pydot


2. 机器硬件aws云服务器：
当前选择的实例类型: p2.xlarge (11.75 ECU, 4 vCPU, 2.7 GHz, E5-2686v4, 61 GiB 内存, 仅限于 EBS)

3. 机器操作系统 Ubuntu：
Deep Learning AMI (Ubuntu) Version 9.0 - ami-8024aaff
Comes with latest binaries of deep learning frameworks pre-installed in separate virtual environments: MXNet, TensorFlow, Caffe, Caffe2, PyTorch, Keras, Chainer, Theano and CNTK. Fully-configured with NVidia CUDA, cuDNN and NCCL as well as Intel MKL-DNN
根设备类型: ebs 虚拟化类型: hvm 已启用 ENA: 是

source activate tensorflow_p36

4. 训练时间
bach_size=128，epoch=8，每个epoch大概用时6分钟，earlystopping于第5个epoach停止训练，5个epoch总共用时大概30分钟。