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

## 言語(categoryの掲示数を取得予定)
- Java
- Ruby
- Python
- Visual Basic

※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="language-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("language-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Java",
      "Ruby",
      "Python",
      "Visual Basic"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100,
          80
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ]
      }
    ]
  },
  "options": {}
});
</script>


## フレームワーク(categoryの掲示数を取得予定)
- Spring boot
- Ruby on Rails
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="framework-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("framework-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Spring boot",
      "Ruby on Rails",
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
        ]
      }
    ]
  },
  "options": {}
});
</script>

## フロントエンド
- Javascript
- JQuery
- CSS
- React
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="frontend-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("frontend-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Javascript",
      "JQuery",
      "CSS",
      "React"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100,
          80
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ]
      }
    ]
  },
  "options": {}
});
</script>

## 開発ツール
- Eclipse
- XCode
- Visual Studio
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="frontend-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("frontend-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Javascript",
      "JQuery",
      "CSS",
      "React"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100,
          80
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB"
        ]
      }
    ]
  },
  "options": {}
});
</script>

## データベース
- MYSQL
- PostgreSQL
- Oracle
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="database-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("database-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "MYSQL",
      "PostgreSQL",
      "Oracle"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56"
        ]
      }
    ]
  },
  "options": {}
});
</script>

## DevOps
- GitLab
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="devops-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("devops-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "GitLab"
    ],
    "datasets": [
      {
        "data": [
          100
        ],
        "backgroundColor": [
          "#FF6384"
        ],
        "hoverBackgroundColor": [
          "#FF6384"
        ]
      }
    ]
  },
  "options": {}
});
</script>

## OS
- Windows
- Mac Os
- Linux(Versionは未定)
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="OperationSystem-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("OperationSystem-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Windows",
      "Mac Os",
      "Linux"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56"
        ]
      }
    ]
  },
  "options": {}
});
</script>

## アルゴリズム

## その他
- Github
- Redmine
- AWS関連
- 人工知能
- 数学
※ chartのコードは別のファイルに割り当てする
<div style="width:100%;">
<canvas id="andsoon-posting-count" height="200"></canvas>
</div>

<script>

new Chart(document.getElementById("andsoon-posting-count"), {
  "type": "pie",
  "data": {
    "labels": [
      "Github",
      "Redmine",
      "AWS関連",
      "人工知能",
      "数学"
    ],
    "datasets": [
      {
        "data": [
          100,
          50,
          100,
          80,
          100
        ],
        "backgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB",
          "yellow"
        ],
        "hoverBackgroundColor": [
          "#FF6384",
          "#4BC0C0",
          "#FFCE56",
          "#36A2EB",
          "yellow"
        ]
      }
    ]
  },
  "options": {}
});
</script>

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
