<div align="center">
  <p align="center">
    중앙대학교 소프트웨어학부 3학년 •
    <a href="https://github.com/CUAI-CAU">CUAI</a> •
    <a href="https://github.com/capstone-privai">capstone-privai</a>
  </p>
</div>
<br/>

안녕하세요, 이정우입니다. LLM 평가와 추론 서빙을 공부하고 있습니다. 같은 모델이라도 측정 조건과 서빙 설정에 따라 점수와 성능이 어떻게 달라지는지를 실제 측정으로 확인하는 일에 관심이 있습니다.

## LLM 평가와 벤치마크

* [**BBQ 편향 벤치마크 재현**](https://github.com/Lee-Jungwoo/bbq-eval-vllm): vLLM 추론 서버로 로컬 모델 24개를 9개 카테고리 31,372문항 규모로 평가했습니다. 'unknown' 선택지를 제거한 강제 선택 조건을 추가하자, 비교 가능한 20개 모델에서 두 조건 간 리더보드 순위 상관은 -0.03이었습니다. (서울대 융합과학기술대학원 인간중심컴퓨팅연구실 하계 연구 인턴, 2026.07~08, 연구실 내부 실험 결과입니다.)
* **DiscrimEval 문항 정제 파일럿**: 70개 시나리오와 3개 인구통계 속성에 대해, 속성 변경이 판단과 규범적으로 무관한 문항인지 LLM 라벨러 3개로 판정했습니다. 전체 Fleiss κ는 0.65, 인종 속성은 0.43이었습니다. (같은 인턴 기간)
* [**Walk-the-Talk**](https://github.com/Lee-Jungwoo/Walk-the-Talk): PubMedQA에서 모델이 설명에 언급한 근거와 실제로 답을 바꾸는 근거가 얼마나 겹치는지를 반사실(counterfactual) 개입으로 측정했습니다. (생성 AI 개론)
* [**name-that-llm**](https://github.com/Lee-Jungwoo/name-that-llm): 짧은 지문의 문체만 보고 18개 LLM 중 작성 모델을 맞히는 분류 문제입니다. TF-IDF n-gram 분류기와 Qwen3-4B LoRA 분류기를 따로 학습한 뒤 보정된 로그 확률을 섞었습니다. (딥러닝 이론 및 실습)

## 평가 데이터와 채점

* [**Mosaic-Credential 평가 데이터**](https://github.com/capstone-privai/promptguard-data): 코딩 에이전트가 외부 LLM으로 보내는 내용에서 비밀값만 가리는 도구의 평가 데이터, 채점, 집계를 맡고 있습니다. 데이터 7종의 정답 비밀 26,778개를 통일된 기준으로 재판정했고, 과제 26개를 조건별 3회씩 실행해 마스킹 적용 시 비밀 노출률이 77%에서 15%로 줄고 과제 성공률이 99%에서 90%로 낮아지는 것을 확인했습니다. (캡스톤디자인 3인 팀, 진행 중. 저장소에는 PromptGuard라는 이름으로 표기되어 있습니다.)

## Linux와 인프라

* [**TigerVNC-Guacamole-Installer**](https://github.com/Lee-Jungwoo/TigerVNC-Guacamole-Installer): Oracle Cloud ARM Ubuntu 22.04 VM에 Nginx, Apache Guacamole, TigerVNC, MariaDB, iptables를 10분 안에 설치하고 설정하는 Bash 스크립트를 작성했습니다.
* **폐쇄망 웹앱 유지보수**: 공군 복무 중 인터넷이 차단된 폐쇄망에서 업무관리 웹앱(Flask)을 1년간 단독으로 유지보수했습니다.
* **커널 모듈 포팅**: 리눅스시스템응용설계 수업에서 연구용 파일시스템 커널 모듈을 Linux 6.6.8에서 7.2.8 API로 포팅하는 팀 과제를 진행하고 있습니다.
* **CUAI 스터디**: 중앙대 AI 학회 CUAI에서 Scaling Book 스터디(roofline 분석, 행렬 샤딩)를 하고 PagedAttention 논문을 리뷰했습니다.
