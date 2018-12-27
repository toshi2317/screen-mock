# S112\_1 担当部署一覧

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | 新規登録 | 表示 | button |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 1 | 新規登録 | 押下でS112\_2 担当部署登録へ画面遷移 |
{% endtab %}
{% endtabs %}

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 2 | 担当部署ID | 更新 | text |
| 3 | 担当部署 | 更新 | text |
| 4 | 検索 | 表示 | button |
| 5 | クリア | 表示 | button |
| 6 | CSV | 表示 | button |
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
      <td style="text-align:left">4</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">
        <p>検索APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値を一覧表示部に表示する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">検索結果をCSVとして出力する</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
**使用API**

**sectionSerch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 担当部署ID | sectionId |
| 3 | 担当部署 | sectionName |
{% endtab %}
{% endtabs %}

### 一覧条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 4 | ID | 表示 | textlink |
| 5 | 担当部署 | 表示 | text |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 詳細条件/仕様 |
| :--- | :--- | :--- |
| 4 | ID | 押下でS112\_3 担当部署編集画面へ遷移 |
| 4 | ID | POPUP表示の場合、押下で親画面に値を引き継ぐ |
{% endtab %}

{% tab title="表示API" %}
**使用API**

**sectionSerch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 4 | ID | sectionId |
| 5 | 担当部署 | sectionName |
{% endtab %}
{% endtabs %}

