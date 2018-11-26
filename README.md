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

#노트2
(11/26)

hukim1112 참고
