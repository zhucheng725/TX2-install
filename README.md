JetPack 3.3 # https://developer.nvidia.com/embedded/jetpack-3_3

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

sudo pip3 install --user --extra-index-url https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu

8.install tensorflow-gpu
bazel:链接：https://pan.baidu.com/s/19T3l_lPSm7jK9ZfjZrj1EA 密码：toqa
tensorflow-gpu-1.9:链接：https://pan.baidu.com/s/1ge7JI9_o3738cR08RxdpJg 密码：zflz

sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer

sudo apt-get install zip unzip autoconf automake libtool curl zlib1g-dev maven -y

download: https://github.com/bazelbuild/bazel/releases/  #bazel-0.23.0-dist.zip

unzip bazel-$bazel-0.23.0-dist.zip -d bazel-dist

sudo chmod -R ug+rwx bazel-dist 
cd bazel-dist
./compile.sh

more details:https://docs.nvidia.com/deeplearning/dgx/install-tf-jetsontx2/index.html

9.error:E: Could not get lock /var/lib/dpkg/lock - open (11: Resource temporarily unavailable)
E: Unable to lock the administration directory (/var/lib/dpkg/), is another process using it?

solve:
sudo rm /var/lib/dpkg/lock
sudo dpkg --configure -a
sudo apt update

error:fatal: Not a git repository (or any of the parent directories): .git
solve: git init

10.install opencv
details:
https://jkjung-avt.github.io/opencv3-on-tx2/
https://www.jianshu.com/p/ae7185d26780
opencv:链接：https://pan.baidu.com/s/1WcklRfx-zRiPBa119yNU0w 密码：rjss
