# S113\_1 担当者一覧

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
| 1 | 新規登録 | 押下でS113\_2 担当者登録画面に遷移 |
{% endtab %}
{% endtabs %}

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 2 | 担当者ID | 更新 | text |
| 3 | 担当部署ID | 更新 | text |
| 4 | 担当者 | 更新 | text |
| 5 | 検索 | 表示 | button |
| 6 | クリア | 表示 | button |
| 7 | CSV | 表示 | button |
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
      <td style="text-align:left">5</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">
        <p>検索APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値を一覧表示部に表示する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">検索結果をCSVとして出力する</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
#### 使用API

**staffSerch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 担当者ID | staffId |
| 3 | 担当部署ID | sectionId |
| 4 | 担当者名 | staffName |
{% endtab %}
{% endtabs %}

### **一覧表示部**

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 8 | 担当者ID | 表示 | textlink |
| 9 | 担当部署ID | 表示 | textlink |
| 10 | 担当者 | 表示 | text |
| 11 | 在籍区分 | 表示 | text |
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
      <td style="text-align:left">8</td>
      <td style="text-align:left">担当者ID</td>
      <td style="text-align:left">押下でS113_3 担当者編集画面を別タブ起動する</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">担当部署ID</td>
      <td style="text-align:left">押下でS112_3 担当部署編集を別タブ起動する</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">在籍区分</td>
      <td style="text-align:left">
        <p>1.在籍 2.休職 3.退職</p>
        <p>リスト値表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

**staffSerch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 8 | 担当者ID | staffId |
| 9 | 担当部署ID | sectionId |
| 10 | 担当者 | staffName |
| 11 | 在籍区分 | type |
{% endtab %}
{% endtabs %}

