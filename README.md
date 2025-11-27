<div align="center">
 

# [<img width="60" height="60" alt="Youtube_logo" src="https://github.com/user-attachments/assets/63b5de86-8a7e-4863-b962-91a9e8e88777" />](https://www.youtube.com/watch?v=q2RPqVL8o3g)  불침번

### 반복되는 야간 근무, 달라진 것을 찾아라! VR 이상 징후 공포게임!

<br>

<table>
  <tr>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/2022eb9e-0a5e-4307-a97e-98164a38f76b" alt="게임 플레이 1" width="100%"/>
      <br/>
      <b>VR Hands 사용</b>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/45dcd774-e7d3-4d75-9f9f-dc71f8f40479" alt="게임 플레이 2" width="100%"/>
      <br/>
      <b>게임 인터렉션</b>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/d6e5eb78-14cb-46c0-8035-3c5267641213" alt="게임 플레이 3" width="100%"/>
      <br/>
      <b>게임 인터렉션2</b>
    </td>
  </tr>
</table>



<br>
<br>

⭐ **무한 루프 공간에서 미묘한 변화를 감지하여 탈출하는 공포 퍼즐 게임**

⭐ **Unity XR을 활용한 몰입감 있는 VR 공포 게임 경험**

⭐ **핸드 트래킹 및 제스처 인식을 통한 직관적인 VR 인터랙션**

</div>

<br>
<br>
<br>


---

</div>

<br>
<br>

## 📋 목차

- [게임 소개](#-게임-소개)
- [프로젝트 개요](#-프로젝트-개요)
- [주요 스크립트](#-주요-스크립트)
  - [YJH Scripts - VR 인터랙션 및 튜토리얼 시스템](#-yjh-scripts---vr-인터랙션-및-튜토리얼-시스템)
- [기술 스택](#-주요-기술-스택)
- [참고사항](#-참고사항)
- [개발자](#-개발자)

<br>
<br>

---

<br>
<br>

## 🎯 게임 소개

**불침번**은 Unity를 활용한 **"8번출구" 게임의 모작 프로젝트**입니다.  
무한 루프 공간에서 미묘한 변화를 감지하여 탈출하는 **VR 공포 퍼즐 게임**을 구현했습니다.  
Unity XR Hands를 활용한 핸드 트래킹 및 제스처 인식 시스템, 튜토리얼 진행 로직, 그리고 VR 인터랙션 시스템으로 몰입감 있는 공포 게임 경험을 제공합니다.

<br>
<br>

---

<br>
<br>

## 📌 프로젝트 개요

| 항목     | 내용                          |
|----------|-------------------------------|
| 유형     | VR 팀 프로젝트                 |
| 기간     | 2025. 04. 16 ~ 2025. 04. 30 (11일)|
| 인원     | 개발자 3명                     |
| 도구     | Unity, Notion                 |

<br>
<br>

---

<br>
<br>

# 📁 YJH Scripts

> 불침번 프로젝트의 YJH 폴더 스크립트 모음입니다.

<br>
<br>

---

## 💻 주요 스크립트

<br>

## 📚 튜토리얼 시스템

<br>

### [`TutorialDialog.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/YJH/TutorialDialog.cs)

**💡 기능**: 튜토리얼 진행 로직 및 제스처 학습 시퀀스 관리

**📌 주요 기능**:
- 순차적인 튜토리얼 진행 로직
- 제스처 학습 시퀀스 관리
- 코루틴을 활용한 순차적 진행

**📌 주요 메서드**:
- `StartTutorial()`: 튜토리얼 시작
- `NextStep()`: 다음 단계로 진행
- `CheckGesture()`: 제스처 학습 확인

**✨ 특징**: 
- 코루틴을 활용한 순차적 튜토리얼 진행
- 제스처 기반 인터랙션 학습

<br>

### [`DialogueManager.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/YJH/DialogueManager.cs)

**💡 기능**: 대화창 UI 표시 및 텍스트 출력 관리

**📌 주요 기능**:
- 대화창 UI 표시 및 관리
- 텍스트 타이핑 효과
- 대화 진행 제어

**📌 주요 메서드**:
- `ShowDialogue(string text)`: 대화창 표시
- `TypeText(string text)`: 텍스트 타이핑 효과
- `CloseDialogue()`: 대화창 닫기

**✨ 특징**: 
- 부드러운 텍스트 출력 효과
- UI/UX 최적화

<br>
<br>

---

<br>
<br>

## 🎮 VR 컨트롤러

<br>

### [`LeftHandMotion.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/YJH/LeftHandMotion.cs)

**💡 기능**: 왼손 제스처 인식 및 이동 제어 (전진/후진/달리기)

**📌 주요 기능**:
- Unity XR Hands를 활용한 핸드 트래킹
- 제스처 인식 (엄지/검지/새끼손가락 인식)
- 이동 제어 (전진/후진/달리기)

**📌 주요 메서드**:
- `DetectGesture()`: 제스처 인식
- `MoveForward()`: 전진 이동
- `MoveBackward()`: 후진 이동
- `Run()`: 달리기

**✨ 특징**: 
- Unity XR Hands를 활용한 핸드 트래킹 구현
- 제스처 기반 이동 시스템
- 자연스러운 VR 이동 경험

<br>

### [`RightHandMotion.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/YJH/RightHandMotion.cs)

**💡 기능**: 오른손 제스처 인식 및 상호작용 제어

**📌 주요 기능**:
- 오른손 제스처 인식
- 상호작용 제어 (물체 잡기, 버튼 누르기 등)
- Unity XR Hands를 활용한 핸드 트래킹

**📌 주요 메서드**:
- `DetectGesture()`: 제스처 인식
- `Interact()`: 상호작용 실행
- `GrabObject()`: 물체 잡기

**✨ 특징**: 
- 직관적인 제스처 기반 상호작용
- UnityEvent를 활용한 유연한 이벤트 시스템

<br>
<br>

---

<br>
<br>

## 🎯 트리거 시스템

<br>

### [`Trigger.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/YJH/Trigger.cs)

**💡 기능**: 플레이어 충돌 감지 및 이벤트 발생

**📌 주요 기능**:
- 플레이어 충돌 감지
- 이벤트 발생 및 처리
- UnityEvent를 활용한 유연한 이벤트 시스템

**📌 주요 메서드**:
- `OnTriggerEnter()`: 충돌 감지
- `OnTriggerExit()`: 충돌 해제
- `InvokeEvent()`: 이벤트 발생

**✨ 특징**: 
- UnityEvent를 활용한 유연한 이벤트 시스템
- 다양한 트리거 시나리오 지원

<br>
<br>

<br>
<br>

---

<br>
<br>

## 🔧 주요 기술 스택

<br>

- 🎮 **Unity 2022.3 LTS**: 게임 엔진
- 🥽 **Unity XR Interaction Toolkit 2.5.4**: VR 인터랙션 시스템
- 🖐️ **Unity XR Hands**: 핸드 트래킹 및 제스처 인식
- 🌐 **Unity OpenXR 1.10.0**: 크로스 플랫폼 VR 지원
- 📝 **TextMeshPro 3.0.6**: UI 텍스트
- 💻 **C# 10.0**: 프로그래밍 언어

<br>
<br>

---

<br>
<br>

## 📝 참고사항

<br>

💡 **VR 아키텍처**
- Unity XR Interaction Toolkit을 활용한 표준화된 VR 인터랙션
- OpenXR을 통한 크로스 플랫폼 VR 지원
- 핸드 트래킹 기반의 자연스러운 제스처 인식

💡 **튜토리얼 시스템**
- 코루틴을 활용한 순차적 튜토리얼 진행
- 제스처 기반 이동 시스템 (엄지/검지/새끼손가락 인식)
- UnityEvent를 활용한 유연한 이벤트 시스템

💡 **VR 컨트롤러**
- Unity XR Hands를 활용한 핸드 트래킹 구현
- 제스처 기반 이동 및 상호작용 시스템
- 자연스러운 VR 이동 경험

💡 **트리거 시스템**
- UnityEvent를 활용한 유연한 이벤트 시스템
- 다양한 트리거 시나리오 지원
- 플레이어 충돌 감지 및 이벤트 발생

<br>
<br>

---

<br>
<br>

<div align="center">

## 👨‍💻 개발자

<br>

**윤종현 (YJH)** - VR 인터랙션 및 튜토리얼 시스템

<br>
<br>

[![GitHub](https://img.shields.io/badge/GitHub-jonghyun109-181717?style=for-the-badge&logo=github)](https://github.com/jonghyun109)

<br>

**📌 모든 스크립트 링크는 위의 GitHub 저장소에서 확인할 수 있습니다.**

</div>

<br>
<br>

