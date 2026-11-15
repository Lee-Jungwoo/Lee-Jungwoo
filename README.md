<div align="center">
  <h3 align="center">
    CAU CSE
  </h3>
</div>
<br/>

안녕하세요, 이정우입니다. LLM Evaluation과 Inference Engineering을 공부하고 있습니다.

## LLM eval

* [**BBQ 편향 벤치마크 재현**](https://github.com/Lee-Jungwoo/bbq-eval-vllm): 로컬 LLM 24개를 vLLM으로 평가하고, '알 수 없음'으로 답을 피하지 못하게 해 점수에 가려져 있던 편향을 드러냈습니다. (서울대 인간중심컴퓨팅연구실 인턴)
* **DiscrimEval 문항 정제 파일럿**: DiscrimEval은 인구통계 속성만 바꿨을 때 판단이 달라지면 차별로 보는데, 속성이 판단과 실제로 관련 있는 문항이 섞여 있을 수 있습니다. LLM 3개로 문항별 관련 여부를 판정해 보니 인종 속성에서 판정이 특히 엇갈려, 기준 자체가 모호한 문항이 있음을 확인했습니다.
* [**Walk-the-Talk**](https://github.com/Lee-Jungwoo/Walk-the-Talk): LLM의 설명은 그럴듯해도 실제 판단 근거와 다를 수 있습니다. 설명에 나온 근거를 하나씩 바꿔 답이 실제로 바뀌는지 확인하는 방식으로 설명의 충실도를 측정했고, 모델의 정답률과 충실도는 다르다는 것을 확인했습니다.
* [**name-that-llm**](https://github.com/Lee-Jungwoo/name-that-llm): 짧은 글의 문체만 보고 18개 LLM 중 어느 모델이 썼는지 맞히는 분류기입니다.

## Projects

* [**Mosaic-Credential 평가 데이터**](https://github.com/capstone-privai/promptguard-data): 코딩 에이전트의 비밀값 마스킹 도구를 평가합니다. 마스킹으로 비밀 노출은 77%에서 15%로 줄고, 과제 성공률은 99%에서 90%로 낮아졌습니다. (캡스톤, 진행 중)

## Linux & Infra

* [**TigerVNC-Guacamole-Installer**](https://github.com/Lee-Jungwoo/TigerVNC-Guacamole-Installer): 클라우드 Ubuntu 서버에 원격 데스크톱 환경을 10분 안에 설치하는 Bash 스크립트입니다.
