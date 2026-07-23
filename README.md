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


결합률과 각 요인의 상관관계 확인

결함률에 영향이 크다고 생각되는 요인 5가지 선별


       '

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
