# SKRRR
영상 및 음성을 활용한 감정 분석 데이팅 어플
# 📎 새로운 인연을 찾아봐!(팀명: HurryUp조)
![image](https://github.com/user-attachments/assets/c2cde952-1e5c-403e-8ee8-d3aca10d0b6a)


## 👀 서비스 소개
* 서비스명: SKRRR
* 서비스설명: Agora, PyTorch를 활용한 호감도 및 감정 분석 데이팅 서비스
<br>

## 📅 프로젝트 기간
2022.08.20 ~ 2022.09.11 (3주)
<br>

## ⭐ 주요 기능
* 기능1: 영상통화 기능 구현
* 기능2: 호감도 분석 음성 모델 제작 
* 기능3: 호감도 분석 영상 모델 제작 
* 기능4: 플러터 
* 기능5: STT기능 구현
<br>

## ⛏ 기술스택
<table>
    <tr>
        <th>구분</th>
        <th>내용</th>
    </tr>
    <tr>
        <td>사용언어</td>
        <td>
            Python, Android Kotlin
        </td>
    </tr>
    <tr>
        <td>프레임워크</td>
        <td>
            PyTorch, Hugging Face, lib, Pyannote
        </td>
    </tr>
    <tr>
        <td>개발도구</td>
        <td>
            Flutter
        </td>
    </tr>
    <tr>
        <td>서버환경</td>
        <td>
           Node.js, Google Cloud
        </td>
    </tr>
    <tr>
        <td>데이터베이스</td>
        <td>
            Firebase, MySQL
        </td>
    </tr>
    <tr>
        <td>협업도구</td>
        <td>
            GIT, GIThub
        </td>
    </tr>
</table>


<br>

## ⚙ 시스템 아키텍처(구조) 예시 
![image](https://github.com/user-attachments/assets/949a7bf0-8af0-4a73-8507-968ebd73534d)

<br>

## 📌 SW유스케이스
![image](https://github.com/user-attachments/assets/f2577b72-8fcf-43f3-b008-adb5907f8ec4)

<br>

## 📌 서비스 흐름도
![image](https://github.com/user-attachments/assets/6e8fd656-e9cb-4c85-b3b9-556570eb753b)
<br>

## 📌 ER다이어그램
![image](https://github.com/user-attachments/assets/638b5735-071d-4b0b-bcb2-2c5e30100737)
<br>

## 🖥 화면 구성

### 홈화면(프로필)/랭킹/Live Chat/이전 통화목록/설정
![image](https://github.com/user-attachments/assets/ad1a9687-96cf-4d3a-833e-6fc99358de02)
![image](https://github.com/user-attachments/assets/93acd331-2b8e-4536-9cb9-035d218faf36)
<br>


## 👨‍👩‍👦‍👦 팀원 역할
<table>
  <tr>
    방찬유: 프로젝트 총괄, 영상통화 기능 구현, DB 설계 및 구축, 클라우드 서버 구축, 프로젝트 발표<br>
    이초원: UI/UX 설계 및 구현, APP 디자인, 화면 렌더링 최적화, DB 연동(MySQL), 시연 영상 제작<br>
    김수민: BERT기반 음성 감정분석모델 학습, 데이터 수집 및 전처리,PM, 산출 문서 작성, PPT 제작<br>
    김형준: TabNet 기반 영상 감정분석모델 학습, 데이터 수집 및 전처리, 모델 DB 연동 및 저장/관리 시스템 구축<br>
    강다연: 회원 더미 데이터 수집 ,데이팅어플 평가 설문지 작성, 회원 취미 기반 질문 데이터 작성 <br>
  </tr>
</table>

## 🤾‍♂️ 트러블슈팅
개념: 문제 해결을 위해 문제의 원인을 논리적이고 체계적으로 찾는 일이며 제품이나 프로세스의 운영을 재개
프로젝트 진행하는 동안 발생했던 이슈 중 가장 기억에 남았던 문제와 해결 프로세스 나열(2~5가지 정도)
  
* 문제1:  음성 분석 모델의 데이터 불균형<br>
문제점: 일부 감정들만 편향적으로 예측 <br>
해결방안: 역번역(영어>프랑스어>영어)방식의 데이터 오버샘플링 진행
 
* 문제2: 영상 모델의 낮은 인식 정확도<br>
 문제점: 객체의 위치, 분류를 동시에 예측한 BlazeFace의 1-stage 방식 <br>
 해결방안: tabNet 2-stage 방식으로 교체(객체 후보영역 찾기>객체 분류 )

* 문제3: Twillo, Vonage 영상 통화 오류<br>
 문제점: 발급된 토큰의 유효기간 만료, 구식 SDK 및 낮은 버전에서만 호환 <br>
 해결방안: Agora로 영상통화 연결, 대시 보드에서 토큰 생성하여 해결 

* 문제4: 오버샘플링 데이터셋 병합 오류<br>
 문제점: 열 구조 및 필드 데이터 타입 불일치로 인해 병합 오류 발생 <br>
 해결방안: 원본 데이터셋과 증강된 데이터셋을 비교하여 구조를 일치시킴 

* 문제5: Flutter화면 렌더링 최적화 이슈<br>
 문제점: 빈번한 위젯 렌더링으로 인한 성능 저하 <br>
 해결방안: const 키워드 및 ListView.builder와 같은 리스트 렌더링 도구 사용








