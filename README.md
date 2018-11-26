# MNIST_with_tensorflow

##아나콘다 이전버전 주소
##https://repo.continuum.io/archive/

##Failed to create start menu 문제
##http://artra.tistory.com/entry/%EC%95%84%EB%82%98%EC%BD%98%EB%8B%A4-Anaconda3-%EC%84%A4%EC%B9%98-%EC%8B%A4%ED%8C%A8-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0-%EB%B0%A9%EB%B2%95


# 노트1

(11/26)
(tensorflow) 가상환경 만들고 jupyter notebook 명령어 써서 들어가도
 import tensorflow as tf 쓸수 없다.
 anaconda prompt 상에서 import tensorflow as tf를 쓸 수 있다고 해도 마찬가지이다.
 
 jupyter notebook 에게 tensorflow를 쓸거라고 kernel을 통해 알려줘야 하기 떄문이다.
 
 anaconda prompt에서
 python -m ipykernel install --user --name = tensorflow
 
 를 통해 ipykernel 라이브러리를 설치한다.
 
 그다음에 
 jupyter notebook을 치고 쥬피터 노트북으로 들어가면 
 New 단축키에 python3과 tensorflow가 함꼐 잇는걸 확인할 수 있다.
 
 (tensorflow) 가상환경을 만들었기 떄문이다.

# 노트2
(11/26)

hukim1112 참고

# 노트3
(11/26)

Tensorflow설치하는법

numpy 나 matplotlib같은 라이브러리는 그냥 pip install 명령어로 설치하면 되지만
tensor는 python 3.7버전에서 그냥 설치가 안되는거 같다

인터넷에 설치하는법이라고 가상환경 (tensorflow) 같은거 만들어서 설치하게 하는건 
jupyter notebook상에서 import tensorflow as tf는 쓸수 있는데 New에서 python3을 통해 tensorflow하는걸 못하게 막는다(노트1 참고)

가상환경없이 (base)에서 직접 tensorflow를 설치해야한다.
https://github.com/tensorflow/tensorflow/issues/17022
주소를 참고

//////////////////////////////////////////////////////////////
(base) C:\Users\James>python --version
Python 3.7.0

(base) C:\Users\James>python -m pip install --upgrade https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-0.12.0-py3-none-any.whl
//////////////////////////////////////////////////////////////

위를 보면 python 이 3.7이고 pip install을 위해 직접 tensorflow 주소를 입력했다. 이건 검색해야하는 듯하다.
https://www.tensorflow.org/install/pip
위의 주소에 가면 각 python버전에 따른 tensorflow pip 있다.


# 노트 4
(11/26)

tensorflow설치했을떄 python에서 import tensorflow as tf 하면 오류나온다

https://github.com/tensorflow/tensorflow/issues/7552

tensorflow버전이 너무 낮거나 하드웨어가 없는ㄴ데 gpu설치한 경우다
https://www.tensorflow.org/install/pip
위의 주소에서 알맞은 tensor설치하고 conda install python=3.6이용하면 된다.

python -m pip install --upgrade https://storage.googleapis.com/tensorflow/windows/cpu/tensorflow-1.12.0-cp36-cp36m-win_amd64.whl

이 명령어로 tensor

