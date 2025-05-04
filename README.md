# JINMOVIE\_VS - TMDB API 기반 영화 검색 사이트

JINMOVIE\_VS는 The Movie Database (TMDB) API를 활용하여 현재 상영 중인 영화 목록을 제공하고, 사용자가 원하는 영화를 검색하여 상세 정보를 확인할 수 있도록 개발된 웹사이트입니다.

### ✨ 주요 기능

* **현재 상영 영화 목록:** TMDB API를 통해 실시간으로 업데이트되는 현재 상영 영화 목록을 메인 페이지에서 확인할 수 있습니다.
* **영화 검색:** 제목 검색 기능을 통해 사용자가 원하는 영화를 빠르게 찾을 수 있습니다.
* **상세 정보 모달:** 각 영화 카드를 클릭하면 영화의 포스터, 제목, 장르, 시놉시스, 그리고 주요 출연진 정보를 담은 상세 정보 모달창이 나타납니다.
* **반응형 디자인:** Bootstrap 프레임워크를 활용하여 다양한 기기 환경에서 최적의 사용자 경험을 제공합니다.
* **캐러셀:** 메인 페이지 상단에 인기 영화 포스터를 슬라이드 형태로 보여줍니다.

### 🛠️ 사용된 기술 스택

* **HTML5:** 웹 페이지의 구조 및 콘텐츠 정의
* **CSS3:** Bootstrap 프레임워크를 활용한 스타일링 및 레이아웃 적용, 사용자 정의 스타일
* **JavaScript (ES6+):**
    * TMDB API 호출 및 데이터 처리 (현재 상영 영화 목록, 영화 검색, 상세 정보, 출연진 정보)
    * 동적인 UI 업데이트 및 사용자 인터랙션 구현 (검색 기능, 모달 창 제어, 캐러셀 동작)
* **Bootstrap 5:** 반응형 웹 디자인 및 UI 컴포넌트 활용
* **TMDB API:** 영화 데이터 (현재 상영 정보, 검색, 상세 정보, 이미지, 출연진 등) 제공

### 🚀 설치 및 실행 방법

1.  **HTML 파일 열기:** 다운로드한 `index.html` 파일을 웹 브라우저 (Chrome, Firefox, Safari 등)로 직접 엽니다.

    ```
    path/to/your/index.html
    ```

    > **주의:** 이 프로젝트는 TMDB API 키를 `config.js` 파일에서 로드하도록 되어 있습니다. API 키를 사용하기 위해서는 다음 단계를 따라 `config.js` 파일을 생성하고 API 키를 설정해야 합니다.

2.  **`config.js` 파일 설정 (필수):**

    * 프로젝트 루트 디렉토리에 `config.js` 파일을 생성합니다.

    * 다음과 같이 TMDB API 키를 변수에 할당합니다. (TMDB API 키를 발급받아야 합니다.)

        ```javascript
        const API_OPTIONS = {
          method: 'GET',
          headers: {
            accept: 'application/json',
            Authorization: 'Bearer YOUR_TMDB_API_KEY' // 여기에 실제 API 키를 입력하세요!
          }
        };
        ```

    * `YOUR_TMDB_API_KEY` 부분을 실제 TMDB API 키로 바꿔주세요. [TMDB 웹사이트](https://www.themoviedb.org/)에서 API 키를 발급받을 수 있습니다.

3.  **웹 브라우저에서 확인:** `index.html` 파일을 웹 브라우저로 열면 현재 상영 중인 영화 목록과 검색 기능을 확인할 수 있습니다.

### 🎬 사용 방법

1.  **현재 상영 영화:** 메인 페이지에 현재 상영 중인 영화들의 카드 목록이 표시됩니다. 각 카드에는 영화 제목, 장르, 간략한 설명, 포스터 이미지가 나타납니다.
2.  **영화 상세 정보:** 보고 싶은 영화 카드의 "View details" 버튼을 클릭하면 해당 영화의 상세 정보 모달창이 열립니다. 모달창에서는 영화 포스터, 제목, 시놉시스, 장르, 그리고 주요 출연진 목록을 확인할 수 있습니다.
3.  **영화 검색:** 페이지 상단의 검색 입력 필드에 찾고 싶은 영화 제목을 입력하고 "검색" 버튼을 누르거나 Enter 키를 누르면 해당 제목을 포함하는 영화 목록이 표시됩니다. 검색어가 없으면 전체 현재 상영 영화 목록이 다시 나타납니다.
4.  **캐러셀:** 메인 페이지 상단의 캐러셀을 통해 인기 영화의 포스터와 간단한 정보를 슬라이드 형태로 감상할 수 있습니다. 좌우 화살표 버튼을 클릭하여 이전/다음 슬라이드로 이동할 수 있습니다.

### 🛠️ 사용된 기술 스택

- **HTML5:** <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5"> 웹 페이지의 구조 및 콘텐츠 정의
- **CSS3:** <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3"> Bootstrap 프레임워크를 활용한 스타일링 및 레이아웃 적용, 사용자 정의 스타일
- **JavaScript (ES6+):** <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
  - TMDB API 호출 및 데이터 처리 (현재 상영 영화 목록, 영화 검색, 상세 정보, 출연진 정보)
  - 동적인 UI 업데이트 및 사용자 인터랙션 구현 (검색 기능, 모달 창 제어, 캐러셀 동작)
- **Bootstrap 5:** <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=flat-square&logo=bootstrap&logoColor=white" alt="Bootstrap"> 반응형 웹 디자인 및 UI 컴포넌트 활용
- **TMDB API:** <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNzzCb4chXJ6SCx-XD-W-X40VcEX5LIsYh4w&s" alt="TMDB API" width="20"> 영화 데이터 (현재 상영 정보, 검색, 상세 정보, 이미지, 출연진 등) 제공

### 📚 demo


![jinMovieSearch](https://github.com/user-attachments/assets/69dc7fc1-dd5d-40a9-8338-a123cf1a0ff1)
![jinMovie](https://github.com/user-attachments/assets/214a94d5-720a-4a4a-94e7-ec971f3a235b)
![jinMovieDetail](https://github.com/user-attachments/assets/7fea77a7-c713-421c-9069-3a84224daace)
