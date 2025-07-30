# ForU(너를 위해) - AI 기반 개인화 단체문자 서비스
> **2025 캡스톤 디자인 프로젝트**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![React](https://img.shields.io/badge/React-18.0+-blue.svg)](https://reactjs.org/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0+-green.svg)](https://spring.io/projects/spring-boot)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-orange.svg)](https://openai.com/)
[![AWS](https://img.shields.io/badge/AWS-EC2%20%7C%20RDS-orange.svg)](https://aws.amazon.com/)


 <img src="https://github.com/brilliant13/portfolio/blob/main/73%E1%84%8C%E1%85%A9_%E1%84%8E%E1%85%AC%E1%84%80%E1%85%A9%E1%84%83%E1%85%A1%E1%84%8B%E1%85%A9.jpg" width="750" alt="best_dao"/> <br>

## 📋 프로젝트 개요

ForU(너를 위해) 는 기업의 영업팀과 마케팅팀을 위한 차세대 AI 기반 개인화 단체문자 발송 플랫폼입니다. 획일적인 단체문자 대신, AI가 각 수신자의 특성과 관계를 분석하여 개인별 맞춤형 메시지를 자동 생성함으로써 고객 참여도와 전환율을 획기적으로 향상시킵니다.

### 🎓 프로젝트 배경 및 목적
현대 디지털 마케팅에서 개인화는 필수 요소가 되었지만, 기존 단체문자 서비스는 모든 수신자에게 동일한 메시지를 발송하여 낮은 참여율과 고객 이탈을 야기합니다. 본 프로젝트는 이러한 문제를 해결하기 위해 **AI 기술을 통한 개인화 메시지**라는 혁신적 접근방식을 제시합니다.

### 🎯 비즈니스 가치

- **고객 참여도 200% 향상**: 개인화된 메시지로 고객의 관심도 극대화
- **업무 효율성 증대**: AI 자동화로 메시지 작성 시간 90% 단축
- **브랜드 차별화**: 고객이 특별함을 느끼는 1:1 커뮤니케이션 경험 제공

## 🎬 시연 영상

### 📱 제품 데모
[![ForU 시연 영상](https://img.youtube.com/vi/07zpJxMxpYQ/0.jpg)](https://youtu.be/e0_yZCZvwcs)


> **2분만에 보는 ForU 핵심 기능**  
> AI 개인화 메시지 생성부터 개인 맞춤화 발송까지 전체 워크플로우를 확인하세요.

## ✨ 핵심 기능

### 🤖 AI 기반 개인화 메시지 생성
- **OpenAI GPT-4** 활용한 고품질 메시지 자동 생성
- 수신자별 개인 정보, 관계, 상황 컨텍스트 반영

### 🎨 AI 이미지 생성
- **DALL-E 3** 기반 맞춤형 시각 콘텐츠 생성
- 메시지 내용과 조화로운 개인화 이미지
- 다양한 스타일과 테마 지원

### 📱 뿌리오(Ppurio) SMS 연동
- 안정적인 대량 문자 발송 인프라
- 실시간 발송 상태 모니터링
- 발송 결과 분석 및 리포팅

## 🏗️ 기술 아키텍처

### Frontend
- **React 18+**: 현대적이고 반응형 사용자 인터페이스
- **현대적 UI/UX**: 직관적인 대시보드 및 워크플로우

### Backend
- **Spring Boot 3.0+**: 견고하고 확장 가능한 REST API 서버
- **Amazon EC2**: 고성능 클라우드 컴퓨팅 환경
- **Swagger/OpenAPI**: 자동화된 API 문서화

### Database
- **MySQL**: 안정적인 관계형 데이터베이스
- **Amazon RDS**: 관리형 데이터베이스 서비스로 고가용성 보장

### External APIs
- **OpenAI GPT-4**: 자연어 생성 및 텍스트 개인화
- **뿌리오(Ppurio) API**: 안정적인 SMS 발송 서비스

### DevOps & Collaboration
- **GitHub**: 소스코드 버전 관리 및 협업
- **CI/CD**: 자동화된 빌드 및 배포 파이프라인

## 🚀 빠른 시작

### 필수 요구사항

- Node.js 18+ 
- Java 17+
- MySQL 8.0+
- AWS 계정
- OpenAI API 키
- 뿌리오 API 키

### 설치 및 실행

#### 1. 저장소 클론
```bash
git clone https://github.com/BestDAOU/Best_front.git
cd Best_front
```

```bash
git clone https://github.com/BestDAOU/Best_back.git
cd Best_back
```

#### 2. 환경 변수 설정
```bash
# Backend 환경 변수 (application.yml)
spring:
  datasource:
    url: jdbc:mysql://54.146.200.149:3306/bestDAOU
    username: ${DB_USERNAME}
    password: ${DB_PASSWORD}

openai:
  gpt.model=gpt-4o
  gpt.api.url=https://api.openai.com/v1/chat/completions
  gpt.api.key=${GPT_API_KEY}
  
ppurio:
  ppurio.api.key=${PPURIO_API_KEY}

# Frontend 환경 변수 (.env)
REACT_APP_API_BASE_URL=http://localhost:8080/api
```

#### 3. Backend 실행
```bash
cd Best_back
./gradlew bootRun
```

#### 4. Frontend 실행
```bash
cd Best_front
npm install
npm start
```

#### 5. 애플리케이션 접속
- Frontend: http://localhost:3000
- Backend API: http://localhost:8080
- API 문서: http://localhost:8080/swagger-ui.html

## 📞 지원 및 문의

### 팀 연락처
- **정 웅** (팀장): [kaka366@naver.com](mailto:kaka366@naver.com)
- **김소룡**: [2071328@hansung.ac.kr](mailto:2071328@hansung.ac.kr)
- **임차민**: [ckals413@naver.com](mailto:ckals413@naver.com)
- **안예찬**: [yes490411@gmail.com](mailto:yes490411@gmail.com)
- **김문권**: [ok63477@gmail.com](mailto:ok63477@gmail.com)
- **유상미** (지도교수): [professor@university.ac.kr](mailto:professor@university.ac.kr)


### 문서 및 리소스
- [API 문서](http://localhost:8080/swagger-ui.html)

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 [LICENSE](./LICENSE) 파일을 참조하세요.

---

**ForU** - 2025 캡스톤 디자인 프로젝트

🎓 **[한성대학교] [컴퓨터공학부]** | 👨‍💻 **BestDAOU: [BestDAOU]** | 📧 **Contact**: 
