<div align="center">
  <p align="center">
    중앙대학교 소프트웨어학부 3학년 •
    <a href="https://github.com/CUAI-CAU">CUAI</a> •
    <a href="https://github.com/capstone-privai">capstone-privai</a>
  </p>
</div>
<br/>

안녕하세요, 이정우입니다. LLM 평가와 추론 서빙을 공부하고 있습니다.

## LLM 평가와 벤치마크

* [**BBQ 편향 벤치마크 재현**](https://github.com/Lee-Jungwoo/bbq-eval-vllm): 로컬 LLM 24개를 vLLM으로 평가하고, '알 수 없음'으로 답을 피하지 못하게 해 점수에 가려져 있던 편향을 드러냈습니다. (서울대 인간중심컴퓨팅연구실 인턴)
* **DiscrimEval 문항 정제 파일럿**: 차별 평가 문항이 타당한지 LLM 3개로 판정해, 판정이 엇갈리는 문항 유형을 찾았습니다.
* [**Walk-the-Talk**](https://github.com/Lee-Jungwoo/Walk-the-Talk): LLM이 설명에서 댄 근거가 실제로 답을 좌우한 근거인지 측정했습니다.
* [**name-that-llm**](https://github.com/Lee-Jungwoo/name-that-llm): 짧은 글의 문체만 보고 18개 LLM 중 어느 모델이 썼는지 맞히는 분류기입니다.

## 평가 데이터와 채점

* [**Mosaic-Credential 평가 데이터**](https://github.com/capstone-privai/promptguard-data): 코딩 에이전트의 비밀값 마스킹 도구를 평가합니다. 마스킹으로 비밀 노출은 77%에서 15%로 줄고, 과제 성공률은 99%에서 90%로 낮아졌습니다. (캡스톤, 진행 중)

## Linux와 인프라

* [**TigerVNC-Guacamole-Installer**](https://github.com/Lee-Jungwoo/TigerVNC-Guacamole-Installer): 클라우드 Ubuntu 서버에 원격 데스크톱 환경을 10분 안에 설치하는 Bash 스크립트입니다.
* **폐쇄망 웹앱 유지보수**: 공군 복무 중 인터넷이 차단된 환경에서 업무용 Flask 웹앱을 1년간 혼자 유지보수했습니다.
* **커널 모듈 포팅**: 연구용 파일시스템 커널 모듈을 Linux 6.6에서 7.2로 포팅하고 있습니다. (수업 팀 과제)
* **CUAI 스터디**: Scaling Book을 공부하고 PagedAttention 논문을 리뷰했습니다.
