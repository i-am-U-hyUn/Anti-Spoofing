# Anti-Spoofing Projects
---

```markdown
# 🧠 Face & ID Matching System (VICLab)

> **AI-powered Identity Verification System**  
> Automated face–ID similarity check and spoofing detection for secure remote authentication.  
> _“We use AI to rebuild trust in the remote era.”_ — Team VICLab

---

## 📘 Overview

비대면 인증이 보편화되면서 **신분증 도용 및 위·변조를 통한 금융사기**가 급증하고 있습니다.  
본 프로젝트는 **AI 기반 얼굴 비교 및 스푸핑 탐지 기술**을 활용하여,  
신분증 사진과 사용자의 실시간 얼굴 영상이 동일인인지 자동으로 검증하는 시스템을 구현합니다.

이 시스템은 금융기관 및 공공서비스의 **비대면 본인인증 정확도**를 높이고,  
고령자·디지털 취약계층 등 **금융소외 계층의 안전한 서비스 이용**을 지원합니다.

---

## 👥 Team Information

| Name | Student ID | 
|------|-------------|
| **김형래** | 2020118135 | 
| **정유현** | 2021110374 | 
| **김민종** | 2020115145 | 
| **문재윤** | 2019116780 | 

**Team:** VICLab  
**Course:** KNU Artificial Intelligence (Prof. Jaehyup Lee)

---

## 🧩 Problem Definition

- 비대면 인증이 확산되면서 **신분증 사진만으로 본인 확인이 불충분**  
- **사람의 눈으로 수작업 검증**하는 기존 방식은 시간·비용 소모가 큼  
- **DeepFake 및 위조 이미지** 등으로 인한 AI 기반 보안 위협 증가  
- 금융사, 공공기관, 원격 의료 등 **신뢰 기반 서비스**에서 높은 정확도의 인증 필요  

---

## 🎯 Project Goals

✅ 신분증에서 얼굴 자동 검출 및 추출  
✅ 실시간 영상에서의 사용자 얼굴 인식 및 포즈 추정  
✅ 두 얼굴 간 유사도 비교 (Cosine Similarity / Euclidean Distance)  
✅ 스푸핑(사진·영상 위조) 탐지로 보안 강화  
✅ 사용자와 기관이 신뢰할 수 있는 AI 인증 프로세스 구현  

---

## 🧠 System Workflow

```

📸 신분증 이미지 입력
↓
🧍 실시간 얼굴 캡처 (좌/우/정면)
↓
🧩 얼굴 특징 추출 (Embedding)
↓
📊 유사도 계산 (FaceNet / ResNet-34)
↓
🧠 스푸핑 탐지 (사진·영상 위조 판별)
↓
✅ 본인 인증 or 🚫 인증 거부

```

---

## ⚙️ Key Technologies

| Category | Tools / Models |
|-----------|----------------|
| **Face Detection** | MediaPipe, YOLOv8 |
| **Face Embedding** | `face_recognition` (ResNet-34 기반) |
| **Similarity Metric** | Cosine Similarity, Euclidean Distance |
| **Spoofing Detection** | CVPR2024 OC-SCMNet, Hyp-OC |
| **Development** | Python 3.10+, OpenCV, PyTorch |
| **Demo Environment** | Google Colab / Jupyter Notebook |

---

## 🧾 Expected Outcomes

| 구분 | 효과 |
|------|------|
| 🔒 보안성 강화 | 얼굴·신분증 이중 인증으로 위조/사기 방지 |
| ⚡ 효율성 향상 | 수작업 검증 자동화로 시간·비용 절감 |
| 🧑‍💻 사용자 편의 | 빠르고 간편한 비대면 본인 확인 |
| 🌍 사회적 가치 | 고령자·취약계층의 금융 접근성 향상 |
| 🏦 산업 확장성 | 금융, 공공, 교육, 헬스케어 등 다방면 적용 가능 |

---

## 📂 Project Materials

> 📎 주요 참고 및 개발 문서 (PDF 포함)

| 파일명 | 내용 요약 |
|--------|------------|
| `VicLab_onepage.pdf` | 프로젝트 요약 및 문제 정의 |
| `회의록.pdf` | 주제 선정 회의 및 역할 분담 기록 |
| `발표ppt.pdf` | 최종 발표 슬라이드 |
| `얼굴_탐지_및_추출.pdf` | 얼굴 검출 / 추출 코드 및 설명 |
| `얼굴유사도검사.pdf` | 얼굴 임베딩 및 유사도 측정 실험 |
| `detect_spoofing_face.pdf` | 스푸핑 탐지 관련 논문 조사 및 구현 정리 |

---

## 📚 References

- [머니투데이: 비대면 신분증 도용 급증 (2024)](https://news.mt.co.kr/mtview.php?no=2024022714025715344)  
- [KBS 뉴스: AI 기반 인증 기술 확산 (2024)](https://news.kbs.co.kr/news/pc/view/view.do?ncd=8030725)  
- [연합뉴스: 디지털 취약계층 보호 필요성 (2024)](https://www.yna.co.kr/view/AKR20241122137500004)  
- [CVPR 2024 - One-Class Face Anti-Spoofing](https://openaccess.thecvf.com/content/CVPR2024/html/Huang_One-Class_Face_Anti-spoofing_via_Spoof_Cue_Map-Guided_Feature_Learning_CVPR_2024_paper.html)

---

## 🌱 Future Work

- Liveness detection 고도화 (blink / motion / depth-based)  
- Flask 또는 Streamlit 기반 Web Demo 개발  
- KYC·AML 금융 규제 대응 자동화  
- 다국어 UI 적용 및 서비스화 검토  

---

## 📢 Slogan

> **"We use AI to rebuild trust in the remote era."**  
> — Team VICLab

---
```

---
