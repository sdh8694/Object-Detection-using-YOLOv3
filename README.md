# Object-Detection-using-YOLOv3

-----

## YOLOv3 Architecture
YOLOv3의 기본 구조는 아래과 같다. (Darknet-53)


![image](https://user-images.githubusercontent.com/58909032/99224594-f7237b80-2829-11eb-8b53-45161737e5ff.png)


## Class Prediction
- Box별 multi-label classification을 사용하여 바운딩 박스가 포함할 수 있는 Class를 예측한다.
- class predicition : softmax를 대신하여 logistic classifier로 대체하였다.

  -> logistic classifier로는 Sigmoid,ReLU,Tanh등이 있다.
- loss fucntion으로는 multi-class classification에서 사용하는 loss함수 대신 binary cross entropy loss를 사용한다.


## Data
COCO 데이터셋을 사용하며, class의 갯수는 80개이다.

## Download
공식홈페이지(https://pjreddie.com/darknet/yolo/) 를 통하여 cfg와 weights 다운받을수 있다.

## Detected image
<div display="inline-block">
<center>
<img src="https://user-images.githubusercontent.com/58909032/99224663-18846780-282a-11eb-86c4-a086cbcd80e1.jpg" display="inline-block" ></img>
<img src="https://user-images.githubusercontent.com/58909032/99222294-998d3000-2825-11eb-92e6-62cb6f88b800.png" display="inline-block" ></img>
</center>
</div>

<div display="inline-block">
<center>
<img src="https://user-images.githubusercontent.com/58909032/99224665-1a4e2b00-282a-11eb-9e52-961cbc9681c3.jpg" display="inline-block" ></img>
<img src="https://user-images.githubusercontent.com/58909032/99222296-9abe5d00-2825-11eb-90b2-011c570723f2.png" display="inline-block" ></img>
</center>
</div>




