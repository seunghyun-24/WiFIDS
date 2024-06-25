# WiFIDS
⋆⁺₊⋆ Wireless Few-shot Intrusion Detection System via Weakly-supervised Learning ⋆⁺₊⋆

---

📢 2024년 1학기 [AIKU](https://github.com/AIKU-Official) 활동으로 진행한 프로젝트입니다. <br />
🎉 2024년 1학기 AIKU Conference 열심히상 수상!

---

## 소개

✅ weakly-supervised learning을 이용한 무선 네트워크 자동 탐지 시스템

무선 네트워크에서 ✨통신의 안전성✨을 보장하려면, ➡️새로운 공격⬅️을 빠르게 감지하여 막아낼 수 있어야 합니다. <br />
현재 침입 탐지 시스템(IDS : Instruction Detection System)은, 지도 학습 방식으로 이루어져 새로운 공격 패턴을 식별하는 능력이 제한적입니다. <br />
최소한의 라벨링 데이터를 사용한 <ins>✔few-shot learning✔</ins>으로 <ins>✔weakly-supervised learning✔</ins>을 진행하여, <br />
다양한 형식의 패킷 기반 공격을 빠르게 탐지할 수 있도록 (더 나아가 새로운 형식의 공격 기법까지!) 새로운 IDS 방식을 보인 ⭐WiFIDS⭐를 구현해보았습니다!


## 방법론

(i) **Few-shot Learning Model 제안** : 새로운 형식의 패킷 기반 무선 공격을 탐지하기 위해 맞춤화된 few-shot 모델입니다. 새로운 공격에 대해 제한된 레이블이 지정된 데이터 문제를 해결하여 실제 네트워크 보안 시나리오에서 작동할 수 있는 것을 목표로 하였습니다. <br />

(ii) **Feasibility 위한 수학적 모델링** : 수학적 모델링을 바탕으로, 제안된 모델의 타당성과 이론적 토대를 입증하고자 노력했습니다. <br />
<p>$\it{\small{\color{#C0C0C0}↳ 여기() 참고}}$</p> 

(iii) **실험/검증** : 다양한 wireless 네트워크 공격에 대한 모델의 효율성을 검증하기 위해 실험을 수행했습니다. 모델이 최소한의 labeled data로 공격 패턴을 탐지 가능함을 보입니다. <br />

(iv) **기존 방법과의 비교/analysis** : 제안한 모델을 기존 패킷 탐지 방법과 비교하여 탐지 정확도, 새로운 공격에 대한 적응성 및 계산 효율성 측면에서 장점을 강조했습니다. <br />

💜 실험, analysis에 대해서는 <a href="https://aiku.notion.site/WiFIDS-29b8250399f640599fafe9f0faa4e992?pvs=4" style="color: #C0C0C0;">aiku 공식 노션</a> 참고

## 환경 설정

- Python ≥ 3.8 
- GPU : GTX4090
  

## 사용 방법
💥 해당 dataset은 메일을 통해 받을 수 있는 자료로, https://icsdweb.aegean.gr/awid/awid3 에서 받아야 합니다. <br />
📁 Dataset을 CSV 폴더 안에 넣어서 해당 실험을 진행할 수 있습니다. <br />
🐍 모든 코드는 ipynb로 구성하였기에, 경로 지정만 수정하여 실행하면 됩니다. <br />
👀 주로 사용한 경로 : /data/experience/wireless/CSV/
🤍 make_dataset, network_preprocess_complete, test 실행 후 result_figure 를 실행하면 figure로 결과를 쉽게 확인할 수 있습니다! 

## 결과
![result1](https://github.com/seunghyun-24/WiFIDS/assets/98291947/33cc6a34-2139-4c20-9c2a-b1b065b83142)
![result2](https://github.com/seunghyun-24/WiFIDS/assets/98291947/091869ab-c888-4e0c-b291-0b842a22ad29)
![result3](https://github.com/seunghyun-24/WiFIDS/assets/98291947/1db11999-1ca2-4918-8b14-b680b49cfbe4)

## 팀원

- [박승현](https://github.com/seunghyun-24?tab=repositories) : 문제정의, 코드 작성, 실험 진행 및 결과 분석
- [김규민] : 코드 작성
- [김상엽] : 코드 작성 
