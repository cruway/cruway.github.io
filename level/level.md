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
<canvas id="canvas" height="300"></canvas>
</div>

<script>

new Chart(document.getElementById("canvas"), {
    type: 'bar',
    data: {
        labels: ['가가가가가가가가가가가가가가', '나나나나나나', '다다다다다다', '라라라라라라', '마마마', '바바바바바바바', '사사사사사사사사', '아아아아아아', '자자자자', '차차차차차차차', '카카카카카카카'],
        datasets: [{
            label: '테스트 데이터셋',
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
            text: '막대 차트 테스트'
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
                    labelString: 'x축'
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
                    labelString: 'y축'
                }
            }]
        }
    }
});

</script>

</script>