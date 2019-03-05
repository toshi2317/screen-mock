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
| 7 | 支払期限日\(From\) | 更新 | date |
| 8 | 支払期限日\(To\) | 更新 | date |
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
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">&#x8868;&#x793A;&#x6761;&#x4EF6;/&#x4ED5;&#x69D8;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>&#x691C;&#x7D22;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x691C;&#x7D22;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x3092;&#x4E00;&#x89A7;&#x8868;&#x793A;&#x90E8;&#x306B;&#x8868;&#x793A;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x30AF;&#x30EA;&#x30A2;</td>
      <td style="text-align:left">&#x691C;&#x7D22;&#x6761;&#x4EF6;&#x90E8;&#x3092;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x306E;&#x72B6;&#x614B;&#x306B;&#x623B;&#x3059;</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">&#x691C;&#x7D22;&#x7D50;&#x679C;&#x3092;CSV&#x3068;&#x3057;&#x3066;&#x51FA;&#x529B;&#x3059;&#x308B;</td>
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
| 7 | 支払期限日\(From\) | paymentDateFrom |
| 8 | 支払期限日\(To\) | paymentDateTo |
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

