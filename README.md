## **패션을 쉽게 MollyMol**


### 🛒 서비스 바로가기

https://mollymol.com/

### **📽️ 시연 영상**

https://drive.google.com/file/d/13Jez_t-zlCY9VO-dskcfzjaCsl4pcMxr/view

### **📽️ 시연 이미지**
![1](https://github.com/user-attachments/assets/beca93ca-68b6-4b55-95c5-9d8ed93d03e4)
![2](https://github.com/user-attachments/assets/dd275067-a169-4f17-ac13-4fb1d682da18)
![3](https://github.com/user-attachments/assets/99d7aab4-bd02-4c7b-9c8a-62c0383dbf4c)
![4](https://github.com/user-attachments/assets/6decaaf6-6081-41a2-94a8-6fbd8921ea62)
![5](https://github.com/user-attachments/assets/ea82e9fd-2983-4470-8848-587fd1ee46f4)

<br>

### **🔖 프로젝트 개요**

---

- 의류 E-commerce
- Fashionista, anyone can be

<br>

### **🎯 목표**

---

- 대용량 트래픽에서 준수한 속도를 유지
- 다수의 트랜잭션에서 동시성 처리 및 일관성 보장

<br>


### 팀 구성

---

**프론트엔드**: 진종환, 최세은

**백엔드**: 이지은, 김정환, 모창일, 이제윤

<br>

### 🧑‍🤝‍🧑 팀 역할

---

![image](https://github.com/user-attachments/assets/97fbfff2-ec90-4350-952c-7050890ae2a7)

<br>

### **📚 기술 스택**

---

![image](https://github.com/user-attachments/assets/e4fbaec5-dde3-48b4-9706-fba3f6fc3f36)

<br>

### **🌏 서버 아키텍쳐**

---

![image](https://github.com/user-attachments/assets/f4ff3c43-79f9-47f4-978a-34aab6a6b43f)

<br>

### 🗺️ ERD

---

![image](https://github.com/user-attachments/assets/d9ddd0fa-e303-4643-a723-b88219edd958)

<br>

### 🗺️ 프론트엔드 아키텍처

---

![image](https://github.com/user-attachments/assets/eda493f6-6069-42db-8ce1-811e84083eb2)


<br>

### 🎞️ 와이어프레임

---

![image](https://github.com/user-attachments/assets/cca35677-13ef-4991-9f9b-ab23a22c79c7)

<br>

### 🧑‍🤝‍🧑 협업

---

![image](https://github.com/user-attachments/assets/c636d5a7-bbc6-4f2f-9f0b-239c29359a7e)


<br>

### **🔗주요 기능**

---

**1️⃣ 회원가입/ 로그인**

- 이메일을 통해 회원 가입 및 로그인을 할 수 있습니다.
- 마이페이지에서 회원 정보를 관리할 수 있습니다.

**2️⃣ 상품 관리**

- 상품 검색 및 필터링 (필터: 카테고리, 색상, 사이즈, 가격 등/정렬: 최신 순, 조회 많은 순, 구매 많은 순  등)
- 상품 상세 페이지 - 이미지, 설명, 리뷰, 재고, 배송 정보 표시
- 상품 등록 -  상품 단건 등록, 상품 다건 (100건 이상부터 1,000,000건 이하) 엑셀로 등록 가능
- 상품 수정 및 삭제

3️⃣ **장바구니**

- 사용자는 상품을 장바구니에 담을 수 있습니다.
- 장바구니에서 옵션 및 수량 변경할 수 있습니다.
- 장바구니 전체 선택, 전체 삭제 할 수 있습니다.

4️⃣ **결제**

- 토스 API를 통해 사용자는 결제를 진행할 수 있습니다.
- 포인트를 사용하여 결제 할 수 있습니다.

**5️⃣ 주문 및 배송 관리**

- 자신의 기본 배송지 설정 및 추가, 변경, 삭제 할 수 있습니다.
- 마이페이지에서 사용자의 주문 내역을 조회할 수 있습니다.

**6️⃣ 리뷰**

- 사용자는 배송완료된 상품의 리뷰를 작성할 수 있습니다.
- 사용자는 리뷰 작성, 수정, 삭제 할 수 있습니다.
- 리뷰에 대한 좋아요 기능을 제공합니다.
- 최근 7일간 누적 좋아요가 많은 인기순위 Top 12를 조회할 수 있습니다.

<br>


---


## **개선사항**

> **Goal**  
> • LCP ≤ 1s / CLS ≈ 0 / 접근성 ≈ 100   

### 3. Product Detail Page

#### 문제상황 1
접근성 기준을 충분히 반영하지 않아 Lighthouse 접근성 점수가 84점으로 나오게 되어 사용자 경험 저하가 우려

#### 해결방안
효율적인 시맨틱 구조, WCAG 2.1 기준 충족, 버튼 및 인터랙션 요소에 aria-label 추가, 이미지에 alt 텍스트 추가, 키보드 탐색 지원, 충분한 색상 대비 제공

#### 결과
Lighthouse의 접근성 점수가 84점에서 100점으로 향상

![image](https://github.com/user-attachments/assets/83ee8906-397d-40fc-bdd8-95fa4f154cd0)

#### 문제 상황 2
페이지 로딩 시 Footer 위치가 콘텐츠 길이에 따라 변동되어 레이아웃이 이동

#### 해결방안
Sticky Footer를 적용해 콘텐츠가 적을 때는 화면 하단에 고정되고 많을 때는 자연스럽게 콘텐츠 흐름을 따라 배치되도록 구조를 개선

#### 결과
CLS가 0.451s에서 0s으로 개선되어 레이아웃 안정성을 확보

![image](https://github.com/user-attachments/assets/d35e7ec8-2749-4767-bbf2-a21833bce247)
![image](https://github.com/user-attachments/assets/32d9559f-3226-479c-b106-54b28373664c)

#### 문제 상황 3
Next.js의 이미지 최적화 기능 대신 자체 이미지 서버의 이미지 최적화 구현으로 LCP 대상 이미지가 저해상도 요청, 명확하지 않은 크기 지정 등으로 인해 브라우저 렌더링을 지연

#### 해결방안
- priority={true}, fetchPriority="high", 명확한 width/height, 고해상도 이미지 요청
- LCP에 중요한 콘텐츠만 먼저 렌더링하고 그 외 내용은 동적 import
- CDN 연결 및 캐싱

#### 결과
LCP가 2.5s에서 0.6s로 개선

![image](https://github.com/user-attachments/assets/8b757973-61ab-4aec-b981-66181e9ff1fa)
![image](https://github.com/user-attachments/assets/1e667b52-622c-4337-91ca-934d84e60e5e)
![image](https://github.com/user-attachments/assets/5b961681-74e1-41f6-9d7b-9378335ee4e7)



<br>


## Git Convention

```bash
ex: [#123] feat: 멤버 조회 시 닉네임 가져오기 비동기 처리

feat: 새로운 기능 추가
fix: 버그 수정
docs: 문서 수정
chore: 그 외 자잘한 작업
test: 테스트 코드
build: 시스템 또는 외부 종속성에 영향을 미치는 변경사항 (npm, gulp, yarn 레벨)
CI: CI관련 설정
style: 코드 의미에 영향을 주지 않는 변경사항 (포맷, 세미콜론 누락, 공백 등)
refactor: 성능 개선
merge: 기능 개발 후 브랜치 병합
docker: 도커 구성
DB: MySQL 데이터베이스 특정 (마이그레이션, 스크립트, 확장 등)
settings: 환경설정
comment : 주석
```

## 폴더 구조

```js
├── app/ # Next.js app router 폴더
│ ├── layout.tsx
│ └── page.tsx
│
├── pages/ # Next.js pages 폴더 (선택적)
│ └── README.md # 해당 폴더의 목적과 역할에 대한 설명
│
├── src/ # 소스 코드
│ ├── app/ # FSD app 폴더 (앱 초기화, 프로바이더 등)
│ │ ├── providers/
│ │ └── authorization/
│ │
│ ├── pages/ # FSD pages 폴더 (페이지 컴포넌트)
│ │ ├── main/
│ │ │ ├── ui/ # 홈 페이지 전용 하위 컴포넌트들
│ │ │ ├── hooks/ # 홈 페이지 전용 커스텀 훅
│ │ │ │
│ │ ├── mypage/
│ │ ├── buy/
│ │ └── product/
│ │
│ ├── entities/ # 비즈니스 엔티티(e.g 유저)
│ │ ├── user/
│ │ │ ├── model/ # 사용자 상태 관리
│ │ │ ├── api/ # 사용자 관련 API 모듈
│ │ │ ├── types/ # 사용자 관련 타입 정의 (TypeScript)
│ │ │ ├── index.ts # 모듈별로 export 정리
│ │ └── product/
│ │
│ ├── widgets/ # 위젯 컴포넌트 (페이지에서 사용하는 재사용 가능한 구성 요소)
│ │ ├── layout/ # 레이아웃 관련 위젯들
│ │ │ ├── Header/ # 헤더 위젯
│ │ │ │ ├── index.ts # 헤더 Export
│ │ │ │ ├── styles.css # 헤더 스타일
│ │ │ │ ├── Header.tsx # 헤더 컴포넌트
│ │ │ │ └── ...
│ │ │ ├── Footer/ # 푸터 위젯
│ │ └── ...
│ │
│ ├── features/ # 기능 단위
│ │ ├── auth/
│ │ │ ├── api/ # 인증 관련 API 통신 모듈
│ │ │ ├── ui/ # 인증 관련 UI 컴포넌트
│ │ │ ├── model/ # 인증 관련 상태 관리
│ │ │ ├── types/ # 인증 관련 타입 정의 (TypeScript)
│ │ │ ├── utils/ # 인증 관련 유틸리티 함수
│ │ ├── cart/
│ │ └── buy/
│ │
│ ├── shared/ # 공통 유틸리티, 컴포넌트, 훅 등
│ │ ├── utils/ # 유틸리티 함수
│ │ ├── hooks/ # 공통 커스텀 훅
│ │ ├── ui/ # 공통 컴포넌트 (Button, Input 등)
│ │ ├── styles/ # 공통 스타일 파일
│ │ ├── types/ # 공통 타입 정의 (TypeScript)
│ │ ├── index.ts # 모듈별로 export 정리
│ │ └── ...
│ └── ...
└── ...
```


