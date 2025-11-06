<div align="center">


# [<img width="60" height="60" alt="Youtube_logo" src="https://github.com/user-attachments/assets/8e31fdca-af1b-4ebc-b2c9-cdb9983454b4" />](https://www.youtube.com/watch?v=q2RPqVL8o3g)  불침번

### 반복되는 야간 근무, 달라진 것을 찾아라! VR 이상 징후 공포게임!

<br>

<table>
  <tr>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/64c29cfb-82ad-4673-aa4f-a88311d303ac" alt="게임 플레이 1" width="100%"/>
      <br/>
      <b>게임 플레이 1</b>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/0b5b7285-9e7d-4609-9c52-a9cff7c269ae" alt="게임 플레이 2" width="100%"/>
      <br/>
      <b>게임 플레이 2</b>
    </td>
    <td align="center" width="33%">
      <img src="https://github.com/user-attachments/assets/c1bce44f-ec46-40e1-92f8-93d5591878ac" alt="게임 플레이 3" width="100%"/>
      <br/>
      <b>게임 플레이 3</b>
    </td>
  </tr>
</table>



<br>
<br>

⭐ **무한 루프 공간에서 미묘한 변화를 감지하여 탈출하는 공포 퍼즐 게임**

⭐ **Unity XR을 활용한 몰입감 있는 VR 공포 게임 경험**

⭐ **동적 이상현상 생성 시스템과 NPC AI를 통한 긴장감 있는 게임플레이**

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
  - [CHM Scripts - 이상현상 및 NPC AI 시스템](#-chm-scripts---이상현상-및-npc-ai-시스템)
  - [ZL Scripts - 유틸리티 라이브러리 및 최적화](#-zl-scripts---유틸리티-라이브러리-및-최적화)
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
Unity XR Hands를 활용한 핸드 트래킹, 동적 이상현상 생성 시스템, NPC AI 추적 시스템, 그리고 분위기 있는 사운드 디자인으로 몰입감 있는 공포 게임 경험을 제공합니다.

<br>
<br>

---

<br>
<br>

## 📌 프로젝트 개요

| 항목     | 내용                          |
|----------|-------------------------------|
| 유형     | VR 팀 프로젝트           |
| 기간     | 프로젝트 진행 중 |
| 인원     | 개발자 3명                     |
| 도구     | Unity, Notion |

<br>
<br>

---

<br>
<br>

# 📁 CHM Scripts

> 불침번 프로젝트의 CHM 폴더 스크립트 모음입니다.

<br>
<br>

---

## 💻 주요 스크립트

<br>

## 🔐 이상현상 시스템

<br>

### [`RoomThreeTrigger.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/RoomThreeTrigger.cs)

**💡 기능**: 플레이어 움직임에 따른 방 색상 변화 이상현상 구현

**📌 주요 기능**:
- 플레이어가 특정 방에 진입 시 방의 색상이 점진적으로 변화
- 코루틴을 활용한 부드러운 색상 전환 효과
- 공포 분위기 연출을 위한 시각적 효과

**✨ 특징**: 
- 시간 기반 이벤트 제어로 자연스러운 전환
- 플레이어의 움직임에 반응하는 인터랙티브한 이상현상

<br>

### [`DoorSoundController.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/DoorSoundController.cs)

**💡 기능**: 플레이어 접근 시 문이 자동으로 열리는 이상현상

**📌 주요 기능**:
- 플레이어가 문 근처에 접근하면 자동으로 문이 열림
- 문 열림 사운드 효과 재생
- Physics.OverlapSphere를 이용한 효율적인 플레이어 감지

**✨ 특징**: 
- 3D 공간 사운드 구현으로 몰입감 향상
- 트리거 시스템으로 인터랙티브한 공포 요소 구현

<br>
<br>

---

<br>
<br>

## 👻 NPC AI 시스템

<br>

### [`Slender_Ctrl.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/Slender_Ctrl.cs)

**💡 기능**: 슬렌더맨 AI - 플레이어 감지 및 추적, 깜빡임 효과

**📌 주요 기능**:
- 플레이어 감지 및 자동 추적 시스템
- 깜빡임 효과로 공포 분위기 연출
- Animator Controller를 통한 복잡한 애니메이션 상태 관리

**📌 주요 메서드**:
- `DetectPlayer()`: Physics.OverlapSphere를 이용한 플레이어 감지
- `ChasePlayer()`: 플레이어 추적 로직
- `BlinkEffect()`: 깜빡임 효과 코루틴

**✨ 특징**: 
- 효율적인 플레이어 감지 시스템
- 부드러운 애니메이션 전환

<br>

### [`CDO_Blood_Ctrl.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/CDO_Blood_Ctrl.cs)

**💡 기능**: 피 묻은 군인 AI - 플레이어 추적 및 크기 증가 효과

**📌 주요 기능**:
- 플레이어 감지 시 자동 추적
- 시간이 지날수록 크기가 증가하는 효과
- 공포 분위기 연출을 위한 시각적 효과

**✨ 특징**: 
- 코루틴을 활용한 시간 기반 크기 변화
- 점진적인 공포감 증가

<br>

### [`CDO_Crying.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/CDO_Crying.cs)

**💡 기능**: 우는 군인 - 주기적 울음소리 및 플레이어 감지 시 기립

**📌 주요 기능**:
- 주기적으로 울음소리 재생
- 플레이어 감지 시 자동으로 기립
- AudioSource를 활용한 3D 공간 사운드 구현

**✨ 특징**: 
- 환경 사운드와 인터랙션 사운드의 조합
- 플레이어 반응에 따른 동적 애니메이션

<br>

### [`CDO_Soldier.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/CHM/CDO_Soldier.cs)

**💡 기능**: 일반 군인 - 경례, 엎드려, 차렷 등 군인 동작 구현

**📌 주요 기능**:
- 다양한 군인 동작 애니메이션 (경례, 엎드려, 차렷)
- Animator Controller를 통한 상태 관리
- 플레이어 감지 시 반응 동작

**✨ 특징**: 
- 복잡한 애니메이션 상태 관리
- 자연스러운 동작 전환

<br>
<br>

---

<br>
<br>

# 📁 ZL Scripts

> 불침번 프로젝트의 ZL 폴더 스크립트 모음입니다.

<br>
<br>

---

## 💻 주요 스크립트

<br>

## 🛠️ 디자인 패턴

<br>

### [`ISingleton.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/ISingleton.cs)

**💡 기능**: 제네릭 싱글톤 패턴 인터페이스 구현

**📌 주요 기능**:
- 제네릭을 활용한 재사용 가능한 싱글톤 패턴
- 타입 안전성 보장
- 확장 메서드를 통한 직관적인 API 제공

**✨ 특징**: 
- 컴포넌트 기반 아키텍처에 최적화
- 메모리 효율적인 구현

<br>
<br>

---

<br>
<br>

## 📦 컬렉션 확장

<br>

### [`ArrayExtensions.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/ArrayExtensions.cs)

**💡 기능**: 배열을 LinkedList로 변환하는 확장 메서드

**📌 주요 메서드**:
- `ToLinkedList<T>()`: 배열을 LinkedList로 변환

**✨ 특징**: 
- 확장 메서드를 통한 직관적인 API
- 제네릭을 활용한 타입 안전성

<br>

### [`LinkedListExtensions.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/LinkedListExtensions.cs)

**💡 기능**: LinkedList의 PopFirst/PopLast 기능 추가

**📌 주요 메서드**:
- `PopFirst<T>()`: 첫 번째 요소 제거 및 반환
- `PopLast<T>()`: 마지막 요소 제거 및 반환

**✨ 특징**: 
- 효율적인 데이터 구조 조작
- 안전한 null 체크

<br>
<br>

---

<br>
<br>

## 🔤 문자열 처리

<br>

### [`CharExtensions.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/CharExtensions.cs)

**💡 기능**: Span을 활용한 고성능 문자열 연결

**📌 주요 기능**:
- `Span<T>`를 사용한 메모리 효율적인 문자열 처리
- 고성능 문자열 연결 연산

**✨ 특징**: 
- 메모리 할당 최소화
- 고성능 문자열 처리

<br>

### [`StringBuilderExtensions.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/StringBuilderExtensions.cs)

**💡 기능**: StringBuilder의 효율적인 Concat 메서드 제공

**📌 주요 메서드**:
- `Concat<T>()`: 제네릭 타입의 효율적인 연결

**✨ 특징**: 
- StringBuilder의 성능 최적화
- 제네릭을 활용한 재사용성

<br>
<br>

---

<br>
<br>

## 🔄 타입 변환

<br>

### [`EnumExtensions.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/EnumExtensions.cs)

**💡 기능**: unsafe 코드를 활용한 Enum↔int 고속 변환

**📌 주요 기능**:
- `unsafe` 코드와 포인터를 활용한 고성능 구현
- Enum과 int 간의 고속 변환

**✨ 특징**: 
- 성능 최적화를 위한 unsafe 코드 활용
- 타입 안전성 보장

<br>

### [`EnumUnion.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/EnumUnion.cs)

**💡 기능**: Enum 변환을 위한 Union 타입 구조체

**📌 주요 기능**:
- Enum 변환을 위한 효율적인 데이터 구조
- 메모리 효율적인 타입 변환

**✨ 특징**: 
- 구조체 기반의 경량 구현
- 타입 변환 성능 최적화

<br>
<br>

---

<br>
<br>

## 🔢 수학 유틸리티

<br>

### [`MathEx.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/MathEx.cs)

**💡 기능**: 각도-라디안 변환 상수 (Deg2Rad, Rad2Deg)

**📌 주요 기능**:
- 각도와 라디안 간의 변환 상수 제공
- 수학 연산 유틸리티

**✨ 특징**: 
- 상수 기반의 효율적인 변환
- 재사용 가능한 유틸리티

<br>

### [`MathFEx.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/MathFEx.cs)

**💡 기능**: float 수학 상수 및 오디오 데시벨 변환 메서드

**📌 주요 기능**:
- float 수학 상수 제공
- 오디오 데시벨 변환 메서드
- 수학 연산 유틸리티

**📌 주요 메서드**:
- `ToDecibel(float linear)`: 선형 값을 데시벨로 변환
- `ToLinear(float decibel)`: 데시벨 값을 선형으로 변환

**✨ 특징**: 
- 오디오 처리에 최적화된 유틸리티
- 정확한 수학 연산

<br>

### [`Main Scene Director.cs`](https://github.com/your-repo/Vigil/blob/main/Assets/Workspace/ZL/Scripts/Main%20Scene%20Director.cs)

**💡 기능**: 메인 씬 디렉터 관리

**📌 주요 기능**:
- 메인 씬의 전반적인 흐름 관리
- 씬 전환 및 이벤트 제어

**✨ 특징**: 
- 싱글톤 패턴 적용 가능한 구조
- 씬 관리의 중앙화

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

💡 **이상현상 시스템**
- 코루틴을 활용한 시간 기반 이벤트 제어
- Physics.OverlapSphere를 이용한 효율적인 플레이어 감지
- 다양한 트리거 시스템으로 인터랙티브한 공포 요소 구현

💡 **NPC AI 시스템**
- Animator Controller를 통한 복잡한 애니메이션 상태 관리
- AudioSource를 활용한 3D 공간 사운드 구현
- 플레이어 반응에 따른 동적 애니메이션

💡 **유틸리티 라이브러리**
- `unsafe` 코드와 포인터를 활용한 고성능 구현
- `Span<T>`를 사용한 메모리 효율적인 문자열 처리
- 제네릭을 활용한 재사용 가능한 유틸리티

💡 **튜토리얼 시스템**
- 코루틴을 활용한 순차적 튜토리얼 진행
- 제스처 기반 이동 시스템 (엄지/검지/새끼손가락 인식)
- UnityEvent를 활용한 유연한 이벤트 시스템

<br>
<br>

---

<br>
<br>

<div align="center">

## 👨‍💻 개발자

<br>

**최현민 (CHM)** - 이상현상 시스템 및 사운드/애니메이션

**이시온 (ZL)** - 유틸리티 라이브러리 및 최적화

**윤종현 (YJH)** - VR 인터랙션 및 튜토리얼 시스템

<br>
<br>

**📌 모든 스크립트 링크는 위의 GitHub 저장소에서 확인할 수 있습니다.**

</div>

<br>
<br>
