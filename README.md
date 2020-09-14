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
- server 123.248.6.100, 80, 8022

# pip3 및 tensorflow 설치
- [Installing TensorFlow For Jetson Platform](https://docs.nvidia.com/deeplearning/frameworks/install-tf-jetson-platform/index.html#benefits)

# ~~미니콘다 설치~~ => agx xavier 에서 공식 지원하지 않음
- [Anaconda doesn’t support aarch64 architecture so you are not able to install it on Jetson Xavie](https://forums.developer.nvidia.com/t/is-it-possible-to-install-anaconda-on-xavier-at-all/83560)
- [c4aarch64_installer-1.0.0-Linux-aarch64](https://qiita.com/PINTO/items/d2054b8ebcbc6c577316)
~~~
su -
wget https://github.com/jjhelmus/conda4aarch64/releases/download/1.0.0/c4aarch64_installer-1.0.0-Linux-aarch64.sh => 미니콘다3 설치
bash c4aarch64_installer-1.0.0-Linux-aarch64.sh => /usr/local/miniconda3/에 설치됨
source ~/.bashrc => 미니콘다 path 등록
conda list => 미 확인시는 nano ~/.bashrc 에서 export PATH="/usr/local/miniconda3/bin:$PATH" 넣어 저장 후 source ~/.bashrc 다시 실행
conda config --set auto_activate_base false => (base)표시 안하기
conda create --name my_env python=2 => 가상환경(my_env) 생성
conda init bash
source ~/.bashrc
conda env list => 가상환경 목록 보기
conda activate my_env => 가상환경 진입
conda deactivate => 가상환경 나오기
conda env remove --name my_env => 가상환경(my_env) 삭제
conda env export --name my_env > environment.yml => 가상환경(my_env) 추출하여 환경을 environment.yml 파일로 저장
conda env create -f ./environment.yml => 저장된 환경파일을 가지고 가상환경 만들기
~~~

