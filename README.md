JetPack 3.3 

chmod +x JetPack-L4T-3.0-linux-x64.run
./JetPack-L4T-3.3-linux-x64_b39.run

$ lsusb #can see NVIDIA Corp

1.cuda 9.0
nvcc --version

2.cudnn 7.0.5
cat /usr/include/cudnn.h | grep CUDNN_MAJOR -A 2

3.tensorrt 4.0 GA

4. can not install anaconda
conda install python=3.6   # 3.7--> 3.6

5.can install tensorflow-gpu=1.10


6.demo
cd NVIDIA_CUDA-9.0_Samples/bin/aarch64/linux/release/
./oceanFFT

cd tegra_multimedia_api/samples/backend
./backend 1 ../../data/Video/sample_outdoor_car_1080p_10fps.h264 H264 --trt-deployfile ../../data/Model/GoogleNet_one_class/GoogleNet_modified_oneClass_halfHD.prototxt --trt-modelfile ../../data/Model/GoogleNet_one_class/GoogleNet_modified_oneClass_halfHD.caffemodel --trt-forcefp32 0 --trt-proc-interval 1 -fps 10

7.
tf:链接：https://pan.baidu.com/s/1t6aEj2iUgcV61J_S2aOKJg 密码：cvl6

ananconda_linux:链接：https://pan.baidu.com/s/1Otj2RnkLUfL0OZGBAcIuUA 密码：qpfr
