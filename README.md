JetPack 3.3 # https://developer.nvidia.com/embedded/jetpack-3_3<br>

chmod +x JetPack-L4T-3.0-linux-x64.run<br>
./JetPack-L4T-3.3-linux-x64_b39.run<br>

$ lsusb #can see NVIDIA Corp<br>

1.cuda 9.0<br>
nvcc --version<br>

2.cudnn 7.0.5<br>
cat /usr/include/cudnn.h | grep CUDNN_MAJOR -A 2<br>

3.tensorrt 4.0 GA<br>

4. can not install anaconda <br>
conda install python=3.6   # 3.7--> 3.6 <br>

5.can install tensorflow-gpu=1.10<br>


6.demo
cd NVIDIA_CUDA-9.0_Samples/bin/aarch64/linux/release/<br>
./oceanFFT<br>

cd tegra_multimedia_api/samples/backend<br>
./backend 1 ../../data/Video/sample_outdoor_car_1080p_10fps.h264 H264 --trt-deployfile ../../data/Model/GoogleNet_one_class/GoogleNet_modified_oneClass_halfHD.prototxt --trt-modelfile ../../data/Model/GoogleNet_one_class/GoogleNet_modified_oneClass_halfHD.caffemodel --trt-forcefp32 0 --trt-proc-interval 1 -fps 10

7.tf:链接：https://pan.baidu.com/s/1t6aEj2iUgcV61J_S2aOKJg 密码：cvl6<br>
ananconda_linux:链接：https://pan.baidu.com/s/1Otj2RnkLUfL0OZGBAcIuUA 密码：qpfr<br>
sudo pip3 install --user --extra-index-url https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu<br>

8.install tensorflow-gpu<br>
bazel:链接：https://pan.baidu.com/s/19T3l_lPSm7jK9ZfjZrj1EA 密码：toqa<br>
tensorflow-gpu-1.9:链接：https://pan.baidu.com/s/1ge7JI9_o3738cR08RxdpJg 密码：zflz<br>

sudo add-apt-repository ppa:webupd8team/java<br>
sudo apt-get update<br>
sudo apt-get install oracle-java8-installer<br>

sudo apt-get install zip unzip autoconf automake libtool curl zlib1g-dev maven -y<br>

download: https://github.com/bazelbuild/bazel/releases/  #bazel-0.23.0-dist.zip<br>

unzip bazel-$bazel-0.23.0-dist.zip -d bazel-dist<br>
sudo chmod -R ug+rwx bazel-dist <br>
cd bazel-dist<br>
./compile.sh<br>
more details:https://docs.nvidia.com/deeplearning/dgx/install-tf-jetsontx2/index.html<br>

9.error:<br>
E: Could not get lock /var/lib/dpkg/lock - open (11: Resource temporarily unavailable)<br>
E: Unable to lock the administration directory (/var/lib/dpkg/), is another process using it?<br>

solve:<br>
sudo rm /var/lib/dpkg/lock<br>
sudo dpkg --configure -a<br>
sudo apt update<br>

error:fatal: Not a git repository (or any of the parent directories): .git<br>
solve: git init<br>

10.install opencv<br>
details:<br>
https://jkjung-avt.github.io/opencv3-on-tx2/<br>
https://www.jianshu.com/p/ae7185d26780<br>
opencv:链接：https://pan.baidu.com/s/1WcklRfx-zRiPBa119yNU0w 密码：rjss<br>

11.TRT version<br>
$ dpkg -l | grep TensorRT<br>


12.ImportError: The _imagingft C module is not installed
```sudo apt-get install libfreetype6-dev
pip uninstall pillow
pip install --no-cache-dir pillow```
