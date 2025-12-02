# Project-CarWiper
## STM32와 아두이노 키트의 부품들을 활용한 자동차 와이퍼 동작 구현
![Image](https://github.com/user-attachments/assets/10680a4e-12d5-466e-bf17-7504e15d32c5)
----------------------------------------------------------------------------------------

### 1. 개요
- **자동차에서 사용되는 와이퍼 기능을 STM32와 아두이노 키트의 부품들을 사용해서 구현한 프로젝트** 
- **조이스틱을 사용하여 서보모터의 속도를 조절과 AUTO모드 설정**
- **AUTO 모드에서는 물 수위센서의 값을 통해서 서보모터의 속도를 조절**

----------------------------------------------------------------------------------------

### 2. 개발 환경 및 도구
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![Keil](https://img.shields.io/badge/Keil-394049?style=flat-square&logo=arm&logoColor=white)

- **MCU : STM32F411RE**
- **입력장치 : 조이스틱, 물 수위센서**
- **출력장치 : 서보모터, LCD**
- **개발방식 : 타이머를 활용한 서보모터 속도 조절, ADC WatchDog를 활용한 물 수위센서의 값에 따라 서보모터 속도 조절**

<img width="1000" height="537" alt="Image" src="https://github.com/user-attachments/assets/20463200-55aa-45bb-934e-1558eb010afa" />

----------------------------------------------------------------------------------------

### 3. 주요 기능
- **조이스틱 : 방향에 따라서 LOW, MIDDLE, HIGH, AUTO 모드 설정**
- **물 수위센서 : AUTO모드 시 설정한 범위에 따라서 LOW, MIDDLE, HIGH 모드 설정**
- **서보모터 : LOW, MIDDLE, HIGH 모드마다 해당 모드에 맞는 속도 출력**
