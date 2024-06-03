# nativeAPP This is a yolov5's Gui program  
1. 새폴더 만들고 CMD 에서 (또는 vscode 터미널에서) 소스코드를 복사한다.
```
git clone 해당 레포 주소
```
2. 새로운 개발환경을 만든다.
```
conda create -n robot python=3.9
```  
3. 콘다 Activate 또는 vscode 에서 개발환경 연결해준다.
```
conda activate robot
```
4. 개발환경 Package 설치
```
pip install -r requirements.txt
```
5. yolov5를 클로닝해온다.(REPO에서는 보이지 않지만)
```
git clone https://github.com/ultralytics/yolov5.git
```

다음과 같은 Tree 구조가 만들어지면 실행
## 폴더구조는  
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/4cf0882b-da39-4433-aa60-f670394588a8)


실행은 windowAPP_feat_Humanoid_tts.py  
## 프로그램 실행 결과  
[ Person ]  
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/17545021-1352-47b0-b869-2cbfb0378f50)  
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/ca639d35-598c-4f0f-b6af-fbcde57910d6)  


[Person 로봇 결과화면](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/130fc6c0-c83e-47c3-ad69-208233c556b3)  

[Bottle 로봇 결과화면](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/1c2c8245-16a9-4b64-9b96-72fdc2797d88)  



## 이 프로그램은 인식 결과에 따라서 휴머노이드 로봇에게 특정 행동을 하도록 한다.  
## TTS를 이용해서 음성 출력을 하도록 하였다. STT는 반대로 음성을 인식하는것을 말함  
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/20f500d1-3dd5-466b-a021-a81e3248ee36)  

## 로봇을 움직이기 위해서는 먼저 SerialPort 객체를 가져와야 한다.  
## PC에 없는 포트를 만들기 위해 cp2104라는 USBtoUART 변환젠더를 사용했고 드라이버가 필요하다.  
```
http://www.iamamaker.kr/ko/tutorials/cp210x-usb-to-uart-%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B2%84-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0/  
```
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/29b97184-7e4d-4330-9854-861f26e583b2)  

로봇을 움직이는 코드는 아두이노의 코드를 파이썬으로 변환 해서 사용하였다.  
![image](https://github.com/jiwon0629/NativeAppYoloCustom_TTS/assets/149983498/3bfcf80a-0418-4486-8ee0-3c48ba4a1b21)







