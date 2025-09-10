# 仕様書評価・承認プロンプト

## 目的
完成した機能仕様書について、レビュー & 承認チェックリストの基準を満たしているかを評価し、チェックリストの更新または改善提案を行う。

## 評価手順
1. 仕様書の「Review & Acceptance Checklist」を確認
2. 各チェック項目について基準適合性を評価
3. 適合している項目は ✅ にマーク
4. 適合していない項目は ❌ にマークし、具体的な改善点を指摘
5. 全体的な品質評価とフィードバックを提供

## 評価観点（Spec Kitテンプレート準拠）

### Content Quality
- **No implementation details (languages, frameworks, APIs)**: 技術スタック、API、コード構造の記述がないか
- **Focused on user value and business needs**: ビジネス要求とユーザーニーズに焦点があっているか
- **Written for non-technical stakeholders**: 非技術者にも理解可能な表現か
- **All mandatory sections completed**: すべての必須セクションが適切に記述されているか

### Requirement Completeness
- **No [NEEDS CLARIFICATION] markers remain**: [NEEDS CLARIFICATION]マーカーが残っていないか
- **Requirements are testable and unambiguous**: 要件が曖昧でなく、検証可能に書かれているか
- **Success criteria are measurable**: 成功基準が測定可能か
- **Scope is clearly bounded**: 機能範囲が明確に定義されているか
- **Dependencies and assumptions identified**: 前提条件や依存関係が明記されているか

## 出力形式

```
# 仕様書評価結果

## Review & Acceptance Checklist

### Content Quality
- [✅/❌] No implementation details (languages, frameworks, APIs)
- [✅/❌] Focused on user value and business needs
- [✅/❌] Written for non-technical stakeholders
- [✅/❌] All mandatory sections completed

### Requirement Completeness
- [✅/❌] No [NEEDS CLARIFICATION] markers remain
- [✅/❌] Requirements are testable and unambiguous
- [✅/❌] Success criteria are measurable
- [✅/❌] Scope is clearly bounded
- [✅/❌] Dependencies and assumptions identified

## 評価サマリー
**総合判定**: [✅ 承認可能 / ⚠️ 修正推奨 / ❌ 要大幅修正]

**主要な問題点**:
- [具体的な問題とその箇所]
- [改善が必要な理由]

**推奨改善アクション**:
1. [具体的な修正提案]
2. [優先順位付きの改善案]

**良い点**:
- [評価できる部分の具体的指摘]
```

## 詳細フィードバック指針

### ❌ 項目がある場合
- **具体的な箇所を指摘**: どの部分が問題かを明示
- **改善案を提示**: 具体的にどう修正すべきかを提案
- **優先度を明示**: クリティカル/重要/軽微の分類

### ✅ 全項目達成の場合
```
🎉 仕様書品質: 承認基準をすべて満たしています！

**実装準備完了**: この仕様書は開発チームに引き渡し可能です。

**特に優秀な点**:
- [具体的に評価できる部分]

**次のステップ**: 
実装タスクの分解と見積もりを行いましょう。
👉 `/plan` コマンドを実行して、開発タスクを生成してください。
```

## 対象仕様書
[ここに評価対象の仕様書全体を貼り付け]

---

**指示**: 上記の仕様書について、レビュー & 承認チェックリストに基づいた評価を実行してください。