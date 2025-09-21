# 📂 GoSung_ROS2

<br>

## 📖 소개 (Introduction)
STM32와 FreeRTOS 기반의 펌웨어부터 ROS2 센서퓨전, 모바일 앱까지, 실외 자율주행 배달 로봇의 핵심 시스템을 개발한 프로젝트입니다.<br>
주요 목표는 교내(인덕대학교) 실외 환경에서 로봇이 안정적으로 주행하고, 다양한 센서 데이터를 융합해 장애물 회피와 경로 생성을 수행할 수 있는 시스템을 구현하는 것입니다.<br>
이 저장소(Repository)는 전체 시스템 중 ROS2, 즉 제어부의 소스 코드를 담고 있습니다.<br><br>
⚠️ 참고: 본 프로젝트는 전문학사 기간 내 개발되었으며, 프로젝트 종료시점에 하드웨어 반납으로 추가 실험 및 장기간 데이터 수집이 불가능했습니다.<br>
본 프로젝트의 실험 결과는 당시 기록된 로그, 녹화 영상, 시뮬레이션을 기반으로 작성되었습니다.<br>

<br>

## ✨ 주요 기능 (Key Features)
- OpenCV를 활용한 카메라 Calibration 수행
- 2D LiDAR-Camera 센서 퓨전 알고리즘 구현

<br>

## 🛠️ 기술 스택 (Tech Stack)
- **Processor / OS**: Notebook (Ubuntu 22.04)
- **Sensor**: `lakibeam1 (2D LiDAR)`, `APC720 (USB Camera)`
- **Language**: `C++`, `Python`
- **Framework/Library**: `ROS2 Humble`, `OpenCV`, `Yolov5`
- **Tools**: `Git`, `GitHub`

<br>

## 👤 기여도 (My Contribution)
본 프로젝트에서 Sensor Fusion 개발 과정을 수행했습니다.
- Camera Calibration
- Yolov5 패키지 분석 및 재사용
- lakibeam1 패키지 분석 및 재사용
- Python 기반 Sensor Fusion 패키지 개발

<br>

## 🚀 시작하기 (Getting Started)
1. 480*640 USB 카메라 연결
2. lakibeam1 LiDAR 연결
3. 객체인식을 위한 yolov5 패키지 detect.py 실행
4. LiDAR 센서 실행을 위한 lakibeam1의 lakibeam1_scan.launch.py 실행
5. 센서퓨전을 위한 sensor_fusion의 sensor_fusion.py 실행
6. 실행 영상 <br>
https://github.com/user-attachments/assets/24dfc483-e2a7-4f59-8c36-abc801f54166

<br>

## 📌 향후 개선 계획 (Future Work)
- 코드 리팩토링 및 모듈별 주석/README 강화
- 시간 동기화 추가
- 객체별 거리 데이터를 활용한 추가 알고리즘 개발

<br>

## 🔧 참고 자료
### YouTube - 프로젝트 최종 데모 영상
https://www.youtube.com/watch?v=ovQ-Pq1NfFU

<br>

- yolov5 패키지의 일부 코드는 아래 프로젝트를 참고하거나 수정하였습니다.  
  [wannn-one/yolov5-ros2 (GitHub)](https://github.com/wannn-one/yolov5-ros2)
  - 라이선스: Apache License 2.0 (LICENSE 파일 포함)

- lakibeam1 패키지의 일부 코드는 아래 프로젝트를 참고하거나 수정하였습니다.  
  [RichbeamTechnology/Lakibeam_ROS2_Driver (GitHub)](https://github.com/RichbeamTechnology/Lakibeam_ROS2_Driver)
  - 라이선스: MIT License (LICENSE 파일 포함)


