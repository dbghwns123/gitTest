# 🐾 반려동물과 함께하는 여행 플랫폼

## 🚀 프로젝트 소개
반려동물을 키우는 사람들을 위한 여행 플랫폼입니다. 🏡🐶🐱
숙박시설 예약부터 주변 산책로, 카페 정보까지 한 번에 확인할 수 있어요!

## 🎯 주요 기능

### 🏠 숙박시설 예약
- 원하는 숙소를 검색하고 예약할 수 있어요.
- 예약 취소 및 변경 기능 제공.
- 호스트가 숙소 정보를 직접 관리 가능.

### 🔎 해시태그 기반 검색 (ElasticSearch 활용)
- 반려동물 동반 가능 숙소, 카페, 산책로를 해시태그로 검색할 수 있어요!
- 인기 해시태그 기반 추천 기능.

### ✍ 후기 및 평점
- 숙소를 이용한 후 후기를 작성하고 평점을 남길 수 있어요.
- 후기 사진 업로드 가능 (AWS S3 활용).

### 👨‍💼 호스트 관리 기능
- 숙박업체가 숙소 정보를 등록하고 수정할 수 있어요.
- 예약 현황을 관리하고, 리뷰에 답변 가능.

## 🛠 기술 스택

### 📌 Backend
- **Spring Boot** - 백엔드 프레임워크
- **Spring Security & JWT** - 인증 및 보안
- **Spring Scheduler** - 자동화 작업 처리
- **Redis** - 캐싱 및 성능 최적화
- **ElasticSearch** - 해시태그 검색 최적화
- **AWS S3** - 이미지 업로드 저장소
- **MySQL** - 데이터베이스

### 📌 Frontend
- **React** - UI 프레임워크
- **TypeScript** - 정적 타입 언어
- **TailwindCSS** - 스타일링

### 📌 DevOps
- **GitHub Actions** - CI/CD 자동화
- **Docker** - 컨테이너화
- **AWS EC2** - 배포 환경

## 📜 API 명세 (예시)
```http
GET /api/v1/hotels?tag=pet_friendly
```
```json
{
  "hotels": [
    {
      "id": 1,
      "name": "멍멍이 호텔",
      "location": "서울 강남구",
      "rating": 4.8,
      "tags": ["pet_friendly", "luxury"]
    }
  ]
}
```

## 📌 프로젝트 구조
```
backend/
├── src/
│   ├── main/
│   │   ├── java/com/pettravel/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── config/
│   │   ├── domain/
│   ├── resources/
│   │   ├── application.yml
frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── styles/
```

## 🎯 목표 및 차별점
✅ 반려동물 동반 여행에 특화된 맞춤형 검색 기능 제공 🐕
✅ 호스트가 직접 숙소 관리를 할 수 있는 편리한 기능 💼
✅ AWS 기반 안정적인 서비스 운영 ☁️
✅ 실시간 인기 해시태그 검색 최적화 🔥

---
💡 **반려동물과 함께 더 즐거운 여행을 떠나보세요!** 🐾✨
