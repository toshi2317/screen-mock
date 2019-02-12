# S113\_2 担当者登録

### 担当者情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 担当者名 | 更新 | text | Y | 50 |
| 2 | 担当部署ID検索 | 表示 | button | Y |  |
| 3 | 担当部署 | 更新 | text | Y |  |
| 4 | 在籍区分 | 更新 | list |  |  |
| 5 | 保存 | 表示 | button |  |  |
| 6 | 戻る | 表示 | button |  |  |
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
      <td style="text-align:left">担当部署ID検索</td>
      <td style="text-align:left">
        <p>常に表示</p>
        <p>押下でS112_1 担当部署一覧画面POPUP表示</p>
        <p>ID押下で当画面遷移、担当部署ID、担当部署名</p>
        <p>自動提案</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">担当部署</td>
      <td style="text-align:left">選択されている部署の[sectionId - sectionName]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">在籍区分</td>
      <td style="text-align:left">
        <p>1.在籍デフォルトセット</p>
        <p>1.在籍 2.休職 3.退職</p>
        <p>リスト表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、登録完了しましたメッセージ表示</p>
        <p>・登録完了しましたメッセージ表示後、S113_3 担当者編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

#### staffSave

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 担当者名 | staffName |
| 3 | 担当部署ID | sectionId |
| 4 | 在籍区分 | type |
{% endtab %}
{% endtabs %}

