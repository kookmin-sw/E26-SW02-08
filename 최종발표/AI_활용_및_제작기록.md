# TrueFrame A0 포스터 — AI 활용 및 제작 기록

- 제작일: 2026-11-04 (Asia/Seoul)
- 기획 기준: 7주차 TrueFrame 문서와 이 대화에서 확정한 발표 대본·추가 요구사항.
- 배경 연도: 발표 공지와 최종 대본에 맞춰 2050년으로 구성.
- 적용 환경: X·Instagram·YouTube 같은 SNS의 기본 기능으로 제안한 미래 콘셉트. 실제 제휴·탑재·구현을 뜻하지 않음.

## AI 활용

- ChatGPT: 기획과 문구 정리, 포스터 구성, 작동 과정·한계 설명, 원본 문서 제작 보조.
- 이미지: OpenAI 기본 이미지 생성 도구(image_gen)를 사용한 신규 생성. CLI/API 우회 방식은 사용하지 않음.
- 이미지 용도: 2050년 출근길 서울 지하철에서 영상 출처를 확인하는 가상 이용자. 실존 인물이나 실제 검증 결과를 표현하지 않음.
- 생성된 장면의 원본 픽셀: 1536 × 1024px.
- 포스터에 배치한 사진의 크기: 252 × 168mm. 실효 해상도 약 154.82 DPI. 원본 사진의 픽셀 수를 늘려 화질이 개선됐다고 주장하지 않음.
- 검증 화면: 사람이 읽을 수 있는 편집 가능한 글자·도형으로 별도 구성한 가상 화면. 확률·정확도 등 검증하지 않은 수치를 사용하지 않음.

## 이미지 생성 프롬프트 원문

Use case: photorealistic-natural. Asset type: a high-resolution central scene photograph for an A0 Korean university future-service research poster, not a whole poster. Generate a brand-new photorealistic editorial image, landscape 3:2 composition, ideally 3072 x 2048 pixels or larger at native generation quality. Scene: Seoul in the year 2050, morning commuter inside a clean believable next-generation metropolitan subway carriage crossing a river, modern green urban skyline and soft morning light through the large window. Subject: fictional Korean office worker around 29 years old, ordinary contemporary smart-casual clothing, seated three-quarter view, thoughtfully looking at a smartphone held naturally in both hands, anatomically accurate hands, realistic skin and fabric. The camera is at an intimate medium distance so the person and phone interaction are immediately readable. Compose the commuter predominantly on the left/center; some depth of train interior and quiet other commuters in background. Keep the smartphone screen angled plausibly, with a simple blurred video thumbnail and small teal visual indicator, absolutely no legible words, no checkmark claiming truth, no real political figures. Convey a calm moment of checking a video's provenance before sharing. Future cues should be subtle and credible: slim glass display, bright accessible transport, no holograms, no cyberpunk, no robots, no futuristic costumes. Palette should complement deep navy, soft blue-grey and restrained turquoise, natural warm daylight. Exceptionally crisp fine details for large-format print, professional documentary photography, grounded and human. Do not include poster titles, labels, borders, logos, charts, text overlays, a poster layout, watermarks, or any typography. The actual Korean verification interface will be added separately as vector text outside this image.

## 생성 후 구성·수정

1. 생성 사진은 포스터의 사용 장면으로 배치하고, 모든 제목·설명·작동 도식·검증 화면을 별도 편집 가능한 글자와 도형으로 제작했다.
2. 발표 흐름에 맞춰 제목·문제·미래 사용 장면·기술 과정·검증 질문·팀 역할의 6개 구역으로 정리했다.
3. SNS 기본 기능이라는 제안, 규제·생성 표시 이후의 관리 과제, 인증 정보가 부족한 경우의 판단 한계를 표시했다.
4. 미래 가설과 현재 기술의 근거를 구분하고, AI 생성 개념 이미지·가상 검증 화면임을 포스터에 표시했다.
5. 인쇄용 PDF의 글자·도식은 벡터로 유지하고 한글·영문 글꼴을 포함했다. 사진과 벡터 색을 CMYK로 변환하고 SWOP 출력 프로필을 포함했다. PDF/X 인증 파일을 주장하지 않는다.
6. SVG와 PowerPoint 편집 원본은 RGB로 보관했다. 인쇄 장비에 따라 색이 달라질 수 있으며 출력 업체의 별도 프로필이 지정되면 그 조건에 맞춰 다시 변환할 수 있다.
7. 실제 동료·멘토 피드백이 제공되지 않아 받은 의견이나 반영 실적을 만들어 넣지 않았다.

## 참고 자료

- C2PA Technical Specification v2.2: https://spec.c2pa.org/specifications/specifications/2.2/specs/C2PA_Specification.html
- U.S. GAO, Science & Tech Spotlight: Malicious Use Of Generative AI: https://www.gao.gov/products/gao-26-108695
- UK AI Security Institute, Managing risks from increasingly capable open-weight AI systems: https://www.aisi.gov.uk/blog/managing-risks-from-increasingly-capable-open-weight-ai-systems
- 팀 저장소: https://github.com/kookmin-sw/E26-SW02-08
- 인쇄용 프로필 출처: ArtifexSoftware/ghostpdl, iccprofiles/default_cmyk.icc (Artifex CMYK SWOP Profile).
