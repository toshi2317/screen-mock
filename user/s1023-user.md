# S102\_3 ユーザー編集

### ユーザー情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ID | 表示 | text | Y |  |
| 2 | メールアドレス | 更新 | text |  |  |
| 3 | 権限 | 更新 | list |  |  |
| 4 | パスワード | 更新 | password |  |  |
| 5 | パスワード変更ボタン | 表示 | check |  |  |
| 6 | 保存 | 表示 | buttton |  |  |
| 7 | 戻る | 表示 | button |  |  |
{% endtab %}

{% tab title="起動時API" %}
**使用API**

**usersearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | userId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | userId |
| 2 | メールアドレス | email |
| 3 | 権限 | userFlag |
| 4 | パスワード | pass |
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
      <td style="text-align:left">3</td>
      <td style="text-align:left">権限</td>
      <td style="text-align:left">
        <p>1:システム管理者</p>
        <p>リスト値表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">パスワード変更ボタン</td>
      <td style="text-align:left">チェックボタン押下で変更不可or可</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、保存APIの返却値をセットしたS102_3 ユーザー編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
**使用API**

**userSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | userId |
| 2 | メールアドレス | email |
| 3 | 権限 | userFlag |
| 4 | パスワード | pass |
{% endtab %}
{% endtabs %}

