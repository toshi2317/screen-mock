# S109\_1 売上一覧

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | 顧客名 | 更新 | text |
| 2 | 電話番号 | 更新 | text |
| 3 | 受注ID | 更新 | text |
| 4 | メールアドレス | 更新 | text |
| 5 | 請求日\(From\) | 更新 | date |
| 6 | 請求日\(To\) | 更新 | date |
| 7 | 支払期限\(From\) | 更新 | date |
| 8 | 支払期限\(To\) | 更新 | date |
| 9 | 区分 | 更新 | check |
| 10 | 検索 | 表示 | button |
| 11 | クリア | 表示 | button |
| 12 | CSV | 表示 | button |
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
      <td style="text-align:left">10</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">
        <p>検索APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値を一覧表示部に表示する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">検索結果をCSVとして出力する</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
**使用API**

salesSearch

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerName |
| 2 | 電話番号 | customerTel |
| 3 | 受注ID | orderId |
| 4 | メールアドレス | customerEmail |
| 5 | 請求日\(From\) | billingDateFrom |
| 6 | 請求日\(To\) | billingDateTo |
| 7 | 支払期限\(From\) | paymentDateFrom |
| 8 | 支払期限\(To\) | paymentDateTo |
| 9 | 区分 | types |
{% endtab %}
{% endtabs %}

### 一覧表示部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 13 | ID | 表示 | textlink |
| 14 | 顧客ID | 表示 | textlink |
| 15 | 受注ID | 表示 | textlink |
| 16 | 顧客名 | 表示 | text |
| 17 | 電話番号 | 表示 | text |
| 18 | メールアドレス | 表示 | text |
| 19 | 請求日 | 表示 | text |
| 20 | 請求金額 | 表示 | text |
| 21 | 区分 | 表示 | text |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 13 | ID | 押下でS109\_3売上編集画面を別タブ起動する |
| 14 | 顧客ID | 押下でS103\_3顧客編集画面を別タブ起動する |
| 15 | 受注ID | 押下でS108\_3受注編集画面を別タブ起動する |
{% endtab %}

{% tab title="表示API" %}
**使用API**

salesSearch

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 13 | ID | salesId |
| 14 | 顧客ID | customerId |
| 15 | 受注ID | orderId |
| 16 | 顧客名 | customerName |
| 17 | 電話番号 | customerTel |
| 18 | メールアドレス | customerEmail |
| 19 | 請求日 | billingDate |
| 20 | 請求金額 | amount |
| 21 | 区分 | types |
{% endtab %}
{% endtabs %}

