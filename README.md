# 👋Hello!
회로 설계와 임베디드 시스템을 학습하는 엔지니어 문성윤입니다.

[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=Gmail&logoColor=white)](mailto:yooni8193@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/yoonisun)

---

## 🚀 About Me
- 🎯 **관심 분야**: Digital Circuit Design, Embedded System, FPGA, PCB Design
- 🔧 **경험 분야**: MCU Firmware, Verilog HDL, UART/I2C/SPI, Circuit Design & Simulation
- 💡 **목표**: 신뢰성 있는 하드웨어를 설계하고 HW/SW 경계를 넘어 시스템을 구현할 수 있는 엔지니어로 성장하는 것입니다.

---

## 🛠 Tech Stack

### Languages & Tools
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-ED8B00?style=flat-square&logo=mathworks&logoColor=white)
![Verilog](https://img.shields.io/badge/Verilog_HDL-001C43?style=flat-square)
![Vivado](https://img.shields.io/badge/Xilinx_Vivado-000000?style=flat-square&logo=xilinx&logoColor=white)
![Assembly](https://img.shields.io/badge/MC68000_Assembly-6E4C13?style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

### Circuit Design & Simulation
![Fritzing](https://img.shields.io/badge/Fritzing-C9002B?style=flat-square)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![PSIM](https://img.shields.io/badge/PSIM-0072C6?style=flat-square)
![LTspice](https://img.shields.io/badge/LTspice-8B0000?style=flat-square)

---

## 📂 Project Experience

### 1. 🛸 바람 외란 하에서 쿼드로터의 데이터 기반 예측 제어
* **진행 기간**: 2025.03 ~ 2025.11 / 2026.05
* **주요 내용**: 비행 데이터를 기반으로 바람 외란 환경에서 쿼드로터의 위치 및 자세를 안정적으로 제어하는 **DeePC(Data-enabled Predictive Control)** 프로젝트
* **사용 기술**: `C` `UART/I2C/SPI` `Arduino` `Fritzing` `KiCad`
* **담당 역할**: 
	* 쿼드로터 회로 설계 및 조립
	* 실험(센서) 데이터 분석 및 센서 펌웨어 개발
* **주요 성과**:
	* **통신 병목 해결 및 신뢰성 확보**: 비행 제어 루프 지연을 해소하기 위해 MCU를 제어부/센서부로 분리하고 I2C Master-Slave 통신 구조를 구현하여 데이터 수신 오류율 0% 달성
	* **온보드 블랙박스 로깅 체계 구축**: 무선 전송 간섭 문제를 극복하기 위해 MicroSD 기반 온보드 로깅 및 버퍼링 방식을 도입, 제어 주기 간섭 없이 실시간 비행 데이터 완벽 수집
	* **커스텀 PCB 재설계**: Fritzing 기반 프로토타입을 KiCad를 이용해 MicroSD 슬롯 및 센서 배치가 최적화된 전용 PCB로 재설계
* **🔗 Repository**: [프로젝트 Repo 링크](#)

---

### 2. 🤖 로봇 제어 및 시뮬레이션 프로그램
* **진행 기간**: 2025.12 ~ 2026.01
* **주요 내용**: Python을 활용하여 로봇의 구조와 상태를 분석하는 여러 시뮬레이션 프로그램을 개발
* **사용 기술**: `Python` `Forward/Inverse kinematics` `Jacobian` `Kalman Filter` `NumPy` `Matplotlib`
* **담당 역할**: 알고리즘 수식 모델링, Python UI/시각화 도구 개발
* **핵심 성과**:
	* Kutzbach Formula 기반 **로봇 자유도 계산기**
	* DH Parameter 기반 **6DOF 로봇 정기구학 시뮬레이션**
	* Jacobian Matrix 기반 **로봇 특이점 탐색 프로그램**
	* Kalman Filter 기반 **IMU + GPS 센서 퓨전 프로그램**
	* Matplotlib / NumPy를 활용한 실시간 시각화
* **🔗 Repository**: [프로젝트 Repo 링크](#)

---

### 3. 🚪 Xilinx Spartan-7 기반 자동문 FSM 제어
* **진행 기간**: 2026.07
* **주요 내용**: Verilog HDL을 이용한 **유한상태머신(Finite-State Machine)** 및 타이머 카운터 기반 디지털 제어 로직 설계
* **사용 기술**: `Verilog HDL` `FSM` `Vivado`
* **담당 역할**: 
	* 순차/조합 논리 회로 모델링
	* Vivado Testbench 작성 및 타이밍 검증
* **주요 성과**:
	* closed / opening / opened / closing 상태 설계
	* 타이머 카운터를 이용한 10초 개폐 및 3초 안전 대기 제어
	* 입력 조건에 따른 Next State Logic 구현
	* Vivado Simulation을 활용한 상태 전이 및 출력 파형 검증
* **🔗 Repository**: [프로젝트 Repo 링크](#)

---

### 4. ⚡ Zynq SoC 기반 PS-PL 연동 복합 제어 시스템
* **진행 기간**: 2026.07
* **주요 내용**: Zynq SoC의 **PS(Processing System)** 와 **PL(Programmable Logic)** 을 AXI GPIO로 연결하여 룰렛 및 반응속도 측정 시스템을 구현
* **사용 기술**: `Verilog HDL` `C` `AXI` `Vivado` `Vitis`
* **담당 역할**: 
	* Vivado 기반 Zynq PS & AXI GPIO IP 블록 디자인
	* 제약 조건(Constraints) 매핑, Vitis C 펌웨어 구현
* **주요 성과**:
	* AMBA AXI 버스 프로토콜 기반으로 PL 영역에 유연하게 주변장치를 배치하여 시스템의 확장성과 유연성을 확보
	* 실시간 이벤트 처리 알고리즘을 HW/SW 통합 구조로 완벽히 검증
* **🔗 Repository**: [프로젝트 Repo 링크](#)

---

### 5. 🔋 PSIM 기반 벅 컨버터 파라미터 최적화 및 리플 저감 설계
* **진행 기간**: 2026.07
* **주요 내용**: 2kW급 강압 DC-DC 벅 컨버터 회로 모델링 및 시뮬레이션 기반 수동 소자 최적화
* **사용 기술**: `PSIM` `LTspice`
* **담당 역할**: 
	* 수식을 기반으로 Duty, Inductance, Capacitance 계산
	* PSIM 회로 모델링 및 파형 분석
* **주요 성과**:
	* 입력 30V → 출력 10V 강압 회로에서 L-C 파라미터 조율 ($L=3.5\mu\text{H}, C=270\mu\text{F}$)
	* 초기 설계 대비 리플 특성을 개선하며 설계 신뢰성 확보
	* **출력 전압 리플 5% 이내** 달성
* **🔗 Repository**: [프로젝트 Repo 링크](#)

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=본인_깃허브_아이디&show_icons=true&theme=transparent&hide_border=true" alt="GitHub Stats" width="45%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=본인_깃허브_아이디&layout=compact&theme=transparent&hide_border=true" alt="Top Languages" width="45%" />
</div>
