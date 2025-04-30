# Project_C
# 🎮 Unity Client Portfolio – Feature Implementation Showcase

> ⚙️ **6개월간 실제 라이브 서비스 프로젝트에서 작업한 Unity 클라이언트 개발 사례**를 정리한 포트폴리오입니다.  
> 이 레포지토리는 개인적으로 수행한 모듈 중심이며, 회사 내부 코드 및 자료는 포함되어 있지 않습니다.

---

## 📌 주요 작업 내용 요약

### ✅ 1. 클라이언트 최적화

- **Mesh Baker** 활용 → 평균 배칭 수 **6000 → 300~500개**로 대폭 감소  
- **Shadow Caster 제거**, **SetPass Call 감소**, **불필요한 Mesh Collider 정리**
- RenderTexture 제거 및 2D Sprite로 대체, `Tag ==` 비교 → `CompareTag()` 변경
- 모델링 LOD 적용 및 폴리곤 수 조정 요청

---

### ✅ 2. 수리 퀴즈 구현

- **마방진 퍼즐**: 직관적인 숫자 UI 기반, 터치 인터랙션 구현
- **스피드 산술 퀴즈**: 난이도에 따라 동적 UI 생성 및 시간 제한 기능 포함

---

### ✅ 3. Plaza Scene – UI 및 이동 구현

- UIManager 및 WarpCheckPopup 구현  
- GateTrigger 스크립트를 통한 포탈 인터랙션 설계

---

### ✅ 4. 엘리베이터 시스템

- `EVRotate.cs` 구현: 회전/이동 애니메이션 및 UI 연동
- 상호작용 기반 승강기 동작 시퀀스 구성

---

### ✅ 5. 방 꾸미기 시스템

- **Easy Grid Builder 커스터마이징**
- 오브젝트 충돌 체크, 투명 소재 변경, 배치 오류 방지 등 버그 수정
- `LookRotation` 활용 벽 배치 정렬 및 UI 배치 개선

---

### ✅ 6. Bus System (NavMesh 기반)

- `MooniBusDriver.cs`로 구현  
- NavMesh Agent 기반 경로 이동, BusStop 태그 처리, 탑승자 동기화 등

---

### ✅ 7. 미니맵 시스템

- 플레이어 마커, 클릭 이동 기능
- 실시간 위치 반영되는 인터랙티브한 UI 구성

---

### ✅ 8. NPC 구조 설계 및 대화 시스템

- **MVC 패턴 적용**, **CSV 기반 대화 관리**
- 선택지 기반 대화, 상태(State) 관리, 랜덤 대화 생성
- Android/iOS 플랫폼별 StreamingAssets 대응 처리
- **로컬라이제이션 적용**, **코루틴 기반 대용량 데이터 처리**

---

### ✅ 9. Addressables 적용 및 경량화

- **씬/리소스를 Addressables로 관리 → 빌드 용량 약 570MB → 200MB**
- InitScene에서 다운로드 UI 구현 및 번들 관리
- `SceneManager.LoadScene()` → `Addressables.LoadAssetAsync()` 전환

---

### ✅ 10. Unity 광고 기능 연동

- Interstitial/Rewarded Ads 구성
- 광고 성공 시 보상 로직 연동 및 오류 처리 분기 구현

---

## 📷 미리보기 이미지

> 일부 주요 작업 장면 미리보기:

---

## 🧠 정리

이 프로젝트는 실제 라이브 서비스 중인 Unity 기반 어플리케이션에 적용된 기능들입니다.  
회사 소속 프로젝트로 전체 코드를 포함할 수는 없지만, 여기 소개된 각 기능들은 **직접 설계/구현/개선한 내용**들입니다.

- ⚙️ **언어**: C#
- 🎮 **엔진**: Unity 2022.x

