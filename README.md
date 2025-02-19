# Go Card GAME ルール

## ゲーム概要
- **プレイヤー数**: 2〜4人 
- **各プレイヤーは以下のカードを受け取ります**:
  - LIFEカード: 5枚
  - 手札: 5枚

## ゲームの目的
- 全員のLIFEを0にする
  - 他のプレイヤーのLIFEカードをすべて削り取ることを目指します。
- 役を作って「Deploy」になる
  - 同じPackageカード（青札）を3枚×2セット揃えることで役を完成させ、「Deploy」と宣言して勝利を目指します。

## セットアップ
1. 残りのカードはテーブル中央に裏向きで積み上げて、山札とします。
2. 各プレイヤーは自分のLIFEカードを正面に並べてください。

## ゲームの進行
1. プレイヤーの順番を決めます。※じゃんけんとかで決めてね。
2. プレイヤーのターンでは次のいずれかのアクションを行います:
   - 山札からカードを1枚引く
   - Actionカードを使用する

### 山札からカードを引いた場合
- 手札が6枚になります。
- Errorカード（赤札）があるなら、そのカードを向かい側の相手に押し付けることが可能です。

### Errorカードの処理
- 同じ種類のPackageカード（青札）を利用すれば、Errorは即時解消可能です。自分のターンで対処しましょう。
- Errorカードを押し付けられたプレイヤーが、自分のターン中にそのErrorに対処できない（しない）場合、LIFEを1つ失います。※LIFEを裏返してください。その際Errorは解消されます。
- 向かい側のプレイヤーがいなくなった場合は、左右のいずれかのプレイヤーにErrorを押し付けてしまいましょう。
  - 同じErrorカードを重ねて、２連続攻撃もできます。

## Actionカード
- 自分のターン中に利用可能です。

1. **debugカード**: 
   - 山札から3枚を見て、好きなカードを手札に加えます。その後手札から不要な1枚を捨てましょう。
   
2. **危険予知カード**: 
   - 場に配置しておけば、Errorを押し付けられた際にErrorを好きな相手に返すことができます。

3. **testingカード**: 
   - 使用すると、どんなErrorも回避できます。

## Deployについて
- 同じPackageカード（青札）を3枚×2セット揃えることで「Deploy」となり勝利します。
- ただし役上がり直前には全員に、LIFEを1つ使って「Pull Request します！」と宣言してください。
- レビュー宣言なしで上がろうとすると「Stealth Commit」扱いとなり、LIFEが削られます。LIFEが０になる場合「Commit Catastrophe」して全員のLIFEが−１になります。

---

楽しんでプレイしてください！ 🎉