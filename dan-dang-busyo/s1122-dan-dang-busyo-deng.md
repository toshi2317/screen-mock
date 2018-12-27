# S112\_2 担当部署登録

### 担当部署情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 担当部署名 | 更新 | text | Y | 100 |
| 2 | 保存 | 表示 | button |  |  |
| 3 | 戻る | 表示 | button |  |  |
{% endtab %}

{% tab title="詳細仕様" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、登録完了しましたメッセージ表示</p>
        <p>・登録完了しましたメッセージ表示後、S112_3 担当部署編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
**使用API**

**sectionSave**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 担当部署名 | sectionName |
{% endtab %}
{% endtabs %}

