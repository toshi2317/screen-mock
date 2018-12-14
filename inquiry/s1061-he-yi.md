# S106\_1 問合履歴一覧

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p>更新</p>
        <p>表示</p>
      </th>
      <th style="text-align:left">部品種類</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">新規登録</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 1 | 新規登録 | 押下でS106\_2 問合履歴登録画面へ遷移 |
{% endtab %}
{% endtabs %}

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 2 | 顧客名 | 更新 | text |
| 3 | 電話番号 | 更新 | text |
| 4 | メールアドレス | 更新 | text |
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

**inquirySearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerName |
| 3 | 電話番号 | customerTel |
| 4 | メールアドレス | customerEmail |
{% endtab %}
{% endtabs %}

### 一覧表示部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p>更新</p>
        <p>表示</p>
      </th>
      <th style="text-align:left">部品種類</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">問合担当者</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">問合電話番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">問合メールアドレス</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">問合題名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 8 | ID | 押下でS106\_3 問合履歴編集画面を別タブ起動する |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

**inquirySearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 8 | ID | inquiryId |
| 9 | 顧客名 | customerName |
| 10 | 問合担当者 | staff |
| 11 | 問合電話番号 | tel |
| 12 | 問合メールアドレス | email |
| 13 | 問合題名 | title |
{% endtab %}
{% endtabs %}

