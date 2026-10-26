# kobun-skill

文化審議会建議「[公用文作成の考え方](https://www.bunka.go.jp/seisaku/bunkashingikai/kokugo/hokoku/93650001_01.html)」（令和4年1月7日）とその解説を、Claude の Agent Skill にまとめたものです。公用文・お知らせ・広報文・通知文を書くときや、表記・用語・文体を校正するときに使えます。

> 本リポジトリは個人が作成した非公式の資料です。文化庁・文化審議会が作成・監修したものではありません。正確な内容は原典を確認してください。

## 含まれるもの

```
skills/kobun-sakusei/
├── SKILL.md              手順、公用文の分類、チェックリスト
└── references/
    ├── hyoki.md          Ⅰ 表記の原則（漢字・仮名、送り仮名186語、外来語、数字、符号）
    ├── yogo.md           Ⅱ 用語の使い方（法令用語、専門用語、外来語、紛らわしい言葉）
    └── bunsho.md         Ⅲ 伝わる公用文のために（文体、見出し、文、構成）
```

## インストール

### Claude Code（プラグインとして）

```
/plugin marketplace add eightman999/kobun-skill
/plugin install kobun@kobun-skill
```

### Claude Code（Skillを直接置く）

```bash
git clone https://github.com/eightman999/kobun-skill.git
cp -r kobun-skill/skills/kobun-sakusei ~/.claude/skills/
```

### Claude.ai / Claude デスクトップ

[Releases](https://github.com/eightman999/kobun-skill/releases) から `kobun-sakusei.zip` を取得し、設定の「Capabilities（機能）」→「Skills」からアップロードします。

## 使い方の例

- 「この案内文を公用文の書き方に直して」
- 「住民向けのお知らせを、解説・広報等の基準でやさしく書いて」
- 「この通知文の表記ゆれと送り仮名を点検して」

## 出典とライセンス

本Skillは、次の資料を加工して作成しました。

- 文化審議会「公用文作成の考え方（建議）」（令和4年1月7日）および「（付）「公用文作成の考え方（文化審議会建議）」解説」（文化庁ウェブサイト https://www.bunka.go.jp/seisaku/bunkashingikai/kokugo/hokoku/93650001_01.html ）を加工して作成

原典は「[文部科学省ウェブサイト利用規約](https://www.mext.go.jp/b_menu/1351168.htm)」に従って利用しています。

本リポジトリの内容は [CC BY 4.0](LICENSE) で公開します。再利用する場合は、本リポジトリと上記の原典の両方の出典を記載してください。
