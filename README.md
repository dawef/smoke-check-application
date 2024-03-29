## 프로젝트 한줄 소개 :
아두이노를 활용한 흡연 탐지 안드로이드 애플리케이션

## 개발 기간 : 
 	
2024.02.01 ~ 2024.03.07


## 개발 동기 :
가족 구성원 중 흡연자가 있어 집에서 흡연 하는 것을 막기 위해 이 프로젝트를 제작하게 되었다.

## 작동 원리 :
아두이노 조도 센서(KY-018)를 통해 센서 값을 지속적으로 받는다.
그 후 블루투스 모듈(HC-06)을 통해 안드로이드와 블루투스 통신을 하며 해당 센서 값을 전달한다.
안드로이드에서는 BluetoothDevice를 통해 아두이노와 연결하고
BluetoothSocket을 통해 socket통신을 시작한다.
BluetoothSocket을 통해 들어온 센서 값을 1초마다 지속적으로 받아 
일정 값에 따라 0~100 (비흡연), 101~300(흡연 의심), 301~ (흡연) 단계를 판단해 안드로이드 스마트폰 화면에 표시한다.

## 시연 화면 :
![image](https://github.com/dawef/smoke-check-application/assets/157953050/65f3bd0c-d877-4ebc-a709-5f981f486cc4)
