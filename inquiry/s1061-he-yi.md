# S106\_1 問合履歴一覧

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">
        <p>&#x66F4;&#x65B0;</p>
        <p>&#x8868;&#x793A;</p>
      </th>
      <th style="text-align:left">&#x90E8;&#x54C1;&#x7A2E;&#x985E;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">&#x65B0;&#x898F;&#x767B;&#x9332;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
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
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">&#x8868;&#x793A;&#x6761;&#x4EF6;/&#x4ED5;&#x69D8;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>&#x691C;&#x7D22;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x691C;&#x7D22;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x3092;&#x4E00;&#x89A7;&#x8868;&#x793A;&#x90E8;&#x306B;&#x8868;&#x793A;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x30AF;&#x30EA;&#x30A2;</td>
      <td style="text-align:left">&#x691C;&#x7D22;&#x6761;&#x4EF6;&#x90E8;&#x3092;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x306E;&#x72B6;&#x614B;&#x306B;&#x623B;&#x3059;</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">&#x691C;&#x7D22;&#x7D50;&#x679C;&#x3092;CSV&#x3068;&#x3057;&#x3066;&#x51FA;&#x529B;&#x3059;&#x308B;</td>
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
| 3 | 電話番号 | tel |
| 4 | メールアドレス | email |
{% endtab %}
{% endtabs %}

### 一覧表示部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">
        <p>&#x66F4;&#x65B0;</p>
        <p>&#x8868;&#x793A;</p>
      </th>
      <th style="text-align:left">&#x90E8;&#x54C1;&#x7A2E;&#x985E;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x62C5;&#x5F53;&#x8005;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x96FB;&#x8A71;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x30E1;&#x30FC;&#x30EB;&#x30A2;&#x30C9;&#x30EC;&#x30B9;</td>
      <td
      style="text-align:left">&#x8868;&#x793A;</td>
        <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x984C;&#x540D;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 8 | ID | 押下でS106\_3 問合履歴編集画面を別タブ起動する |
| 9 | 顧客名 | 押下でS103\_3 顧客編集画面を別タブ起動する |
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

