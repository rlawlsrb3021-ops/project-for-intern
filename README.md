어떤 요인에 따라 제품의 결함률에 영향이 가는지 알아 보고자 함 

다양한 요인에 따라 제품불량 발생
이 프로젝트는 케글에서 가져온 데이터를 바탕으로 각 요인에 따라 얼마나 결함이 나타나는지 알아보고자함 그에 따른 영향이 큰 요인을 개선하기 위함

이 데이터(총 3240개의 생산 조건)에서 각 공정, 제품가격 외 11가지 에 따른 결과 (불량률 불량 상태 품질 점수) 분석

요인 후보
ProductionVolume', 'ProductionCost', 'SupplierQuality',
'DeliveryDelay',   'MaintenanceHours',
'DowntimePercentage', 'InventoryTurnover', 'StockoutRate',
'WorkerProductivity', 'SafetyIncidents', 'EnergyConsumption',
'EnergyEfficiency', 'AdditiveProcessTime', 'AdditiveMaterialCost',

에너지 효율과 에너지 소비는 겹치는 범위로 판단 에너지 소비로 에너지 관련 부분 변수 설정
생산 비용은 결함률과 관계없을 것으로 판단 제외


결합률과 각 요인의 상관관계 확인

결함률에 영향이 크다고 생각되는 요인 7가지 선별
근거:대부분의 변수의 상관관계 절대값이 0.01 ~ 0.03사이에 포진 그 중 대부분이 0.01 ~ 0.013사이에 밀집 0.01 ~ 0.013사이 변수들은 하나의 대표 변수를 뽑고 그 변수를 분석한 결과가 나머지 변수와 비슷한 양상을 보일 것으로 예상

7가지 변수와 결함률 비교
적층 공정시간과 결합률의 관계
시간과 결함률의 관계를 시각적으로 보기 위해 산점도 그래프 사용
변수 변화에 따른 결함률에 미치는 영향이 미미
또한 각 구간별 결함률 수치 차이도 미미

다른 상관계수가 작은 변수들도 비슷한 양상을 보일 것으로 판단 
각 변수들이 영향을 개별적으로 주는 영향이 적다고 판단 

따라서 변수들의 조합에 따라 결함률에 어떤 영향을 주는지 분석




       

```text
Manufacturing_Defect_Analysis
│
├── README.md
├── Manufacturing_Analysis.ipynb
├── data
│   └── manufacturing_data.csv
└── images
    ├── correlation.png
    └── defect_analysis.png
```
