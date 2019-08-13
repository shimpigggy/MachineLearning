## Anaconda 설치 ------ python 3.7 version 

https://www.anaconda.com/distribution/

<br/>

## CUDA v9.0 설치 exe(local)

https://developer.nvidia.com/cuda-toolkit-archive
<br/>환경변수가 제대로 설치 되었나 확인
<br/>시스템 환경변수 편집 -> 고급 -> 환경변수 클릭 -> CUDA_PATH
<br/>


## cuDNN 설치

**cuDNN v7.0.5 for CUDA 9.0**으로 설치
<br/>https://developer.nvidia.com/rdp/cudnn-archive
<br/>압축파일을 압축 해제후 cuda 폴더에 들어가보면 **bin/include/lib 3개의 파일**이 있다
<br/>이 세개 폴더에 **CUDA_PATH 경로의 폴도에 추가: ctrl+c/ ctrl+v**

<br/>

## Anaconda를 이용해 Tensorflow 설치

conda에 가상 환경 생성
<br/>**conda create -n NAME pip python=3.5** /*환경 만들기(python 3.5) -> y/n 나오면 y 누를것.*/
<br/>**activate NAME** /*환경 활성화*/
<br/>**python -m pip install --upgrade pip** /*일단 pip 를 업그레이드 시켜준다.*/
<br/>**pip install --ignore-installed --upgrade tensorflow-gpu==1.12.0** /*텐서플로우 GPU 버전 설치*/
<br/><br/><br/>


## 참고 사이트

https://devyurim.github.io/python/tensorflow/2018/04/30/tensorflow-1.html
