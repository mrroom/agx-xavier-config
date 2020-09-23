# agx-xavier-config

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

