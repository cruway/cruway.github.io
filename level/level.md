---
title: "level"
permalink: /level
layout: single
author_profile: true
---
### レベル
※ 棒グラフ追加予定(設計中)

## 全体技術ステータス
※ こっちはchart raderを利用して作る予定
<div style="width:100%;">
<canvas id="programmer-ability" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("programmer-ability"), {
  "type": "radar",
  "data": {
    "labels": [
      "技術力",
      "コミュニケーション",
      "集中力",
      "学習力",
      "熱情",
      "体力",
      "敏捷性"
    ],
    "datasets": [
      {
        "label": "シムウクのステータス",
        "backgroundColor": "rgba(255,99,132,0.2)",
        "borderColor": "rgba(255,99,132,1)",
        "pointBackgroundColor": "rgba(255,99,132,1)",
        "pointBorderColor": "#fff",
        "pointHoverBackgroundColor": "#fff",
        "pointHoverBorderColor": "rgba(255,99,132,1)",
        "data": [
          78,
          78,
          90,
          79,
          96,
          77,
          80
        ]
      }
    ]
  },
  "options": {
    "responsive": true, 
    "scale": {
          "ticks": {
              "stepSize": 10,
              "beginAtZero":true,
              "min": 0,
              "max": 100
          }
      }
  }
});
</script>

## 設計

## 言語
- Java
- Ruby
- Python
- Visual Basic

## フレームワーク
- Spring boot
- Ruby on Rails

## フロントエンド
- Javascript
- JQuery
- CSS

## 開発ツール
- Eclipse
- XCode
- Visual Studio

## データベース
- MYSQL
- PostgreSQL
- Oracle

## DevOps
- gitLab

## アルゴリズム

## その他
- Github
- Redmine
- AWS関連
- 人工知能
- 数学

```mermaid
graph TD
  A --> B
  C --> D
```

<div style="width:100%;">
<canvas id="canvas2" height="300"></canvas>
</div>

<script>

new Chart(document.getElementById("canvas2"), {
    type: 'bar',
    data: {
        labels: ['aaaa', 'bbbb', 'cccc', 'dddd', 'eeee', 'ffff', 'gggg', 'hhhh', 'iiii', 'gggg', 'jkkkk'],
        datasets: [{
            label: 'test dataset',
            data: [
                10,
                3,
                30,
                23,
                10,
                5,
                15,
                20,
                13,
                5,
                9
            ],
            borderColor: "rgba(255, 201, 14, 1)",
            backgroundColor: "rgba(255, 201, 14, 0.5)",
            fill: false,
        }]
    },
    options: {
        responsive: true,
        title: {
            display: true,
            text: 'chart test'
        },
        tooltips: {
            mode: 'index',
            intersect: false,
            callbacks: {
                title: function(tooltipItems, data) {
                    return data.labels[tooltipItems[0].datasetIndex];
                }
            }
        },
        hover: {
            mode: 'nearest',
            intersect: true
        },
        scales: {
            xAxes: [{
                display: true,
                scaleLabel: {
                    display: true,
                    labelString: 'x'
                },
                ticks: {
                    autoSkip: false
                }
            }],
            yAxes: [{
                display: true,
                ticks: {
                    suggestedMin: 0,
                },
                scaleLabel: {
                    display: true,
                    labelString: 'y'
                }
            }]
        }
    }
});
</script>
