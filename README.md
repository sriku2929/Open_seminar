# Open_seminar

オープンゼミ用の教材です。前半はTitanicを使って機械学習の流れを解説し、後半は参加者のみなさんにSpaceship Titanicに取り組んでもらいます。

## フォルダ構成

```
Open_seminar/
├── titanic/                 # 解説用（Titanic）
│   ├── train.csv            # 学習データ（891行・Survivedあり）
│   └── test.csv             # 予測用データ（418行）
├── spaceship-titanic/       # 演習用（Spaceship Titanic）
│   ├── train.csv            # 学習データ（8,693行・Transportedあり）
│   ├── test.csv             # 予測用データ（4,277行）
│   └── sample_submission.csv
└── README.md
```

## データの読み込み（Google Colab）

クローンしなくても、次のコードでGitHubから直接読み込めます。

```python
import pandas as pd

BASE = "https://raw.githubusercontent.com/sriku2929/Open_seminar/main"

# Titanic
train = pd.read_csv(f"{BASE}/titanic/train.csv")
test = pd.read_csv(f"{BASE}/titanic/test.csv")

# Spaceship Titanic
sp_train = pd.read_csv(f"{BASE}/spaceship-titanic/train.csv")
sp_test = pd.read_csv(f"{BASE}/spaceship-titanic/test.csv")
```

## データの出典

- [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic)（Kaggle）
- [Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic)（Kaggle）

予測結果を提出してスコアを確認したい場合は、Kaggleアカウントを作成し、各コンペに参加登録してください。
