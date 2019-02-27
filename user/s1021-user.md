# S102\_1 ユーザー一覧

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | 新規登録 | 表示 | button |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 1 | 新規登録 | 押下でS102\_2 ユーザー登録画面へ遷移 |
{% endtab %}
{% endtabs %}

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 2 | ユーザーID | 更新 | text |
| 3 | メールアドレス | 更新 | text |
| 4 | 権限 | 更新 | list |
| 5 | 検索 | 表示 | button |
| 6 | クリア | 表示 | button |
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
      <td style="text-align:left">権限</td>
      <td style="text-align:left">
        <p>1:システム管理者</p>
        <p>リスト値表示</p>
      </td>
    </tr>
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
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
**使用API**

**usersearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | ユーザーID | userId |
| 3 | メールアドレス | email |
| 4 | 権限 | userFlag |
{% endtab %}
{% endtabs %}

### 一覧表示部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 5 | ID | 表示 | textlink |
| 6 | メールアドレス | 表示 | text |
| 7 | 権限 | 表示 | text |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 5 | ID | 押下でS102\_3 ユーザー編集画面に遷移 |
| 7 | 権限 | リスト値=1:システム管理者 表示 |
{% endtab %}

{% tab title="表示API" %}
**使用API**

**usersearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 5 | ID | userId |
| 6 | メールアドレス | email |
| 7 | 権限 | userFlag |
{% endtab %}
{% endtabs %}

