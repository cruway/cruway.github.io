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
<canvas id="programmer-ability" height="300"></canvas>
</div>

<script>

new Chart(document.getElementById("programmer-ability"), {
    type: 'radar',
    data: {
        labels: ['理解力', '技術力', '集中力', '熱情', '学習力', 'コミュニケーション'],
        datasets: [{
            label: 'シム ウクの能力値',
            data: [
                90,
                80,
                70,
                83,
                90,
                80
            ],
            borderColor: "rgba(255, 201, 14, 1)",
            backgroundColor: "rgba(255, 201, 14, 0.5)",
            fill: true,
            lineTension: 0
        }]
    }
});
</script>

## 進捗のchart数値を取得してどうやって表現するのか？

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
