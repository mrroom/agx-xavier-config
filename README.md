# agx-xavier-config

- [Install Jetson Software with SDK Manager](https://docs.nvidia.com/sdk-manager/install-with-sdkm-jetson/index.html)
- [Fan Mode Control](https://docs.nvidia.com/jetson/l4t/index.html#page/Tegra%2520Linux%2520Driver%2520Package%2520Development%2520Guide%2Fpower_management_jetson_xavier.html%23wwpID0E03M0HA)
- FAN 모드 및 온도 체크
~~~
  # FAN 모드 조회
  sudo /usr/sbin/nvpmodel -q
  
  # FAN 모드 변경
  sudo /usr/sbin/nvpmodel -d <fan_mode>(quiet or cool)
  
  # 
  sudo apt-get install lm-sensors
  sudo sensors
  thermal-fan-est-virtual-0
  Adapter: Virtual device
  temp1:        +33.6°C 
~~~

- [우분투 NVMe M.2 ssd 사용하기](https://promobile.tistory.com/371)
- [ASUS공유기 포트포워딩](https://little-kid.tistory.com/8)
- [ASUS공유기 SSH활성화](https://lightinglife.tistory.com/144)

# pip3 및 tensorflow 설치
- [Installing TensorFlow For Jetson Platform](https://docs.nvidia.com/deeplearning/frameworks/install-tf-jetson-platform/index.html#benefits)
- [Ubuntu에서 Python 버전을 변경하는 방법](https://codechacha.com/ko/change-python-version/)

# ~~미니콘다 설치~~ => agx xavier 에서 공식 지원하지 않음 : Miniforge 사용
- [Python 딥러닝 환경 구성하기](https://kynk94.github.io/devlog/post/jetson-nano-conda)
- [Miniforge](https://github.com/conda-forge/miniforge)
- [[Jupyter Lab & Notebook] 설치, 실행 및 원격 접속 방법](https://jm4488.tistory.com/46)

# pytorch 설치
- [Jetson AGX Xavier Development Kit Setup for Deep Learning (Tensorflow, PyTorch and Jupyter Lab) with JetPack 4.x SDK](https://rahulvishwakarma.wordpress.com/2020/06/23/jetson-agx-xavier-development-kit-setup-for-deep-learning-tensorflow-pytorch-and-jupyter-lab-with-jetpack-4-x-sdk/)
- [[Jetson AGX Xavier] pytorch, tensorflow, pillow, scipy 등 설치](https://m.blog.naver.com/tbvj5914/221631290399)
- [Installing MindsDB](https://docs.mindsdb.com/Installing/)
- [From sources:tokenizers](https://github.com/huggingface/tokenizers/tree/master/bindings/python)
- [파이토치(pytorch) 시작하기/파이토치 튜토리얼](https://m.blog.naver.com/keum_zz6/221316995599)
- [모두를 위한 딥러닝 시즌2 !!](https://deeplearningzerotoall.github.io/season2/lec_pytorch.html)
- [예제로 배우는 파이토치(PYTORCH)](https://tutorials.pytorch.kr/beginner/pytorch_with_examples.html)
- [[PyTorch로 시작하는 딥러닝 기초] 05. Logistic Regression](https://wegonnamakeit.tistory.com/44)
- [REALTIME MOBILE OBJECT DETECTOR IN XAMARIN.ANDROID](https://geeks.ms/xamarinteam/2019/07/04/realtime-mobile-object-detector-in-xamarin-android/)

