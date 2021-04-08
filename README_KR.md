# Synapse-AML-Battery-Forecasting

## Introduction

Azure ML의 주요 기능을 데모/실습을 통해 파악하고, 배터리 수명 관련 공개데이터를 이용해 Forecasting을 수행해봅니다.

## Strategy

- 실습은 AzureML의 Compute Instance로 활용해서 실습하는 것으로 하되,
- 데모는 VSCode도 확인해봅니다.
  - [VSCode로 CI에 직접 붙는 것](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-set-up-vs-code-remote?tabs=extension)
  - [VSCode의 Remote connection 기능](https://code.visualstudio.com/docs/remote/ssh#:~:text=To%20connect%20to%20a%20remote%20host%20for%20the,select%20the%20type%20manually.%20...%20More%20items...%20)
  - [VSCode에서 extension 이용해 Azure ML 활용하는 부분](https://docs.microsoft.com/en-us/azure/machine-learning/tutorial-setup-vscode-extension)
  - [VSCode에서 SDK로 제출하는 부분](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-configure-environment#local)

## Scope

- 기본 실습내용 진행
  - Azure ML Workspace 만들기 (공용)
  - Compute Instance (개별), Computer Cluster 생성하기
  - Notebooks - Terminal에서 `git clone https://github.com/azure/machinelearningnotebooks`
  - 첫번째 실험 (local)
  - MNIST/sklearn 학습 (remote) /배포

- 데이터 준비/가공
  - 원 데이터 + 가공된 데이터: Blob에 public으로 업로드
  - 가공 로직: Synapse에 import할 .ipynb
  - Azure ML에 Dataset으로 등록 로직: Azure ML CI에서 활용할 .ipynb

- 실험 수행 - 모델 생성
  - Automated ML / UI 활용

- 모델 평가
  - explanation 분석하는 부분에 시간 할애

- 모델 패키지/배포
  - UI에서 수행

- 모델 사용
  - SDK/API 사용하여 모델 consume, 시각화: Synapse 또는 Azure ML CI에서 활용할 .ipynb
  - Synapse에서 Power BI로 모델 consume
  - [Power BI Desktop에서 모델 consume](https://docs.microsoft.com/en-us/power-bi/connect-data/service-aml-integrate?context=azure/machine-learning/context/ml-context)

## Contribute

TODO: Explain how other users and developers can contribute to make your code better.

If you want to learn more about creating good readme files then refer the following [guidelines](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme?view=azure-devops). You can also seek inspiration from the below readme files:

- [ASP.NET Core](https://github.com/aspnet/Home)
- [Visual Studio Code](https://github.com/Microsoft/vscode)
- [Chakra Core](https://github.com/Microsoft/ChakraCore)