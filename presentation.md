---
marp: true
paginate: true
header: Github : gbdngb12
footer: 김동건 포트 폴리오
theme: marp-black-white
---

# `$ whoami`

<div class="colwrap">
<div class="left">

<div class="colwrap2">
<div class="left">

## 자기 소개
![h:200](./image/dong.png)

</div>
<div class="right inverted">

#
#
#
#
안녕하세요.
문제를 **주도적으로 찾고**,
**주어진 문제를 끈기 있게 해결**하는 김동건 입니다!

</div>
</div>

## 보유 기술

- **`C`**/ **`C++`** / **`Python`** / `HTML/CSS/JS` / `Java/Kotlin`
- **`x86`, `ARM64`, `MIPS64`**, `s390x`
- `docker`, `Git`

</div>

<div class="right inverted">

## 학력 및 이력
- 부경대학교 **컴퓨터공학전공** 
    (2018.03 ~ 2025.02 졸업 예정)
- KITRI **BoB 취약점 분석 12기**
    (**컴파일러 최적화 취약점 분석 PM**)
- **`codeinject` 
도구 프로젝트** 및 **세미나 발표**
- **CTF 대회** 출전 
    (`UofTCTF 2024`, `Insomni'hack`, 
    `hspace CTF`)

## [GitHub Link(gbdngb12)](https://github.com/gbdngb12)

</div>
</div>

---

# `$ Compiler Optimization Vulnerability Analysis`

## 컴파일러 최적화 취약점 분석 프로젝트 요약

| 항목&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | 내용 |
|:-----|:-----|
| **프로젝트 기간** | 2023.09 ~ 2023.12 (4개월) |
| **진행 배경** | 컴파일러 최적화 과정은 <span style="color:#3550d8;font-weight:bold;">매우 복잡</span>, 의도하지 않은 <span style="color:red;font-weight:bold;">취약점</span> 분석</span> |
| **역할** | **PM**, 프로젝트 총괄 및 발표 (총 6명) |
| **기술적 핵심 내용** | 컴파일러 **Fuzzer 개발** 및 **CodeQL**, 최적화 버그 <span style="color:red;font-weight:bold;">취약점</span> 연계 |
| **프로젝트 성과** | 컴파일러 버그 31건, 학술대회 논문 2개, Stealth Backdoor 시나리오 연구, PoC 3개 개발, CodeQL Query 9개 개발 |
| **프로젝트 링크** | [GitHub](https://bobpiler.github.io/compiler-optimization-vulnerability-explorations/) |

<!-- 음 핵심 정리 내용
- 프로젝트 내용
- 프로젝트 기간
- 프로젝트 진행 배경
- 프로젝트내의 역할
- 프로젝트 기술적 핵심 내용
- 프로젝트 성과
- 프로젝트 링크 -->

---

# `$ Compiler Optimization Vulnerability Analysis`

## 프로젝트 핵심 내용 : `Fuzzer`

`*CG: Code Generator, *Arch: Architecture, *CO: Compile Options`
<p align="center">
  <img height="350px" src="image/fuzzer.png">
</p>

CG에서 생성된 코드가 **Executor**에서 컴파일 및 실행, **Analyzer, Validator**에서 버그 탐지

---

# `$ Compiler Optimization Vulnerability Analysis`

## 프로젝트 성과 : `Conference Paper Submission, Vulnerability PoC Using Compiler Bugs, CodeQL Query`

학술대회 논문 투고, 컴파일러 최적화 버그가 취약점으로 연결 될 수 있음을 증명하는 PoC 개발, 컴파일러 최적화 버그를 탐지하는 CodeQL Query 개발

<p align="center">
<image src="image/paper_poc_codeql.png" height=500px></image>
</p>


---

# `$ Compiler Optimization Vulnerability Analysis`

## 프로젝트 성과 : `Stealth Backdoor Scenario`

<span style="color:red;font-weight:bold;">악의적인 공격자</span>가 **컴파일러 최적화 버그**를 이용해서 <span style="color:#3550d8;font-weight:bold;">오픈소스</span>에 **코드를 삽입**할 경우 
특정한 <span style="color:#3550d8;font-weight:bold;">컴파일러, 아키텍쳐, 최적화 옵션</span>에서 <span style="color:red;font-weight:bold;">취약점</span>을 유발하는 시나리오 연구

![alt text](image/stealth_backdoor_scenario.png)


---

# `$ Development codeinject Tool`

## `codeinject` 도구 개발 프로젝트 요약

| 항목&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | 내용 |
|:-----|:-----|
| **프로젝트 기간** | 2023.05 ~ 2023.06 (1개월) |
| **진행 배경** | **ELF, PE**, 객체지향 **C++** 학습 및 악성코드 도구 개발 |
| **역할** | 개인 프로젝트 |
| **기술적 핵심 내용** | ELF, PE 구조, C++, Linux/Windows Loader의 역할, 클래스 다이어그램 |
| **프로젝트 성과** | **`codeinject` 도구**, 부산대-부경대 **세미나 발표** |
| **프로젝트 링크** | [GitHub](https://github.com/gbdngb12/codeinject.git) |

---

# `$ Development codeinject Tool`


<div class="colwrap3">
<div class="left">

## 프로젝트 핵심 내용 : `Class Diagram`,

![h:450](image/class_diagram.png)

</div>
<div class="right inverted">

## `Principle Study`

![pe inject](image/pe_inject.png)

</div>
</div>

## 

---

# `$ Development codeinject Tool`

## 프로젝트 성과 : `codeinject Tool`, `Seminar Presentation`

<div class="colwrap4">
<div class="left">

# 
#
#
#
![h:450](image/codeinject.png)

</div>
<div class="right inverted">

#
#
#
#
![h:450](image/semina2.jpg)

</div>
</div>

---

# `$ CTF`


## 지속적인 CTF 대회 출전 : `UofTCTF 2024`, `Insomni'hack`, `hspace CTF`
<div class="colwrap4">
<div class="left">

#
#
#
#

<p align="center"> 
<image src="image/CTF.png"></image>

올해에 열린 **CTF대회에 출전**함으로써 **`pwnable` 기술**을 공부하며, <span style="color:red;font-weight:bold;">취약점</span>을 찾고 **expolit**할 준비를 하고 있습니다 !

</div>
<div class="right inverted">

#
#
#
<p align="center"> 
<image height=450px src="image/dream_hack.png"></image>
</p>
</div>
</div>



---

# `Future Plan`

## `1. Study Binary Fuzzing`
바이너리 Fuzzing에 대한 공부 및 Fuzzing 진행

## `2. Analysis 1-Day Vulnerability`
기존 취약점 1-Day 분석 진행

## `3. Find Real World Major Program Vulnerability`
리얼 월드에서 메이저 프로그램의 취약점 찾기


<div class="colwrap5">
<div class="left">

#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
## 김동건
### Email : gbdngb12@naver.com
### GitHub : https://github.com/gbdngb12

</div>
<div class="right inverted">

#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
### 꾸준하게 하자.

</div>
</div>


<!-- #### 꾸준하게 하자. -->


<!-- # `$ Compiler Optimization Vulnerability Analysis`

## 프로젝트 성과 : `CodeQL Query for Compiler Bug Detection`

컴파일러 <span style="color:#3550d8;font-weight:bold;">최적화 버그</span>를 탐지하는 **`CodeQL Query`**

<image align="center" src="image/codeql.png" height=400px>

</image> -->




<!-- 
# `$ Compiler Optimization Vulnerability Analysis`

## 진행 배경

<p align="center">
  <img height="300px" src="image/compiler_optmization_vulnerability.png">
</p>

- **컴파일러 최적화 과정**은 <span style="color:#3550d8;font-weight:bold">매우 복잡</span>하며, <span style="color:#3550d8;font-weight:bold">다양한 아키텍쳐</span>를 지원합니다.
- 이러한 이유로 **컴파일러 최적화 버그**가 발생할 수 있습니다.
- 이는 **곧 바이너리의** <span style="color:red;font-weight:bold;"> 잠재적인 보안 취약점</span>으로 **연결** 될 수 있으므로 프로젝트를 진행했습니다.

--- -->
<!-- 
# `$ Compiler Optimization Vulnerability Analysis`

## 프로젝트 핵심 내용 : `Overview`

<p align="center">
  <img height="250px" src="image/comp2.png">
</p>

- 컴파일러 <span style="color:#3550d8;font-weight:bold;">최적화 버그</span>를 탐지하는 **Fuzzer를 개발**하여 **컴파일러 최적화 버그 탐지 및 분석**
- 컴파일러 <span style="color:#3550d8;font-weight:bold;">최적화 버그</span>와 **바이너리 취약점 연계**
    - <span style="color:#3550d8;font-weight:bold;">CodeQL</span>을 활용한 취약점 진단
    - <span style="color:#3550d8;font-weight:bold;">컴파일러 최적화버그</span>가 <span style="color:red;font-weight:bold;">취약점</span>을 유발 할 수 있음을 증명하는 <span style="color:red;font-weight:bold;">PoC</span> 개발

--- -->