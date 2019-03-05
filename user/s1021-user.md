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
| 7 | メール配信 | 表示 | button |
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
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x6A29;&#x9650;</td>
      <td style="text-align:left">
        <p>1:&#x30B7;&#x30B9;&#x30C6;&#x30E0;&#x7BA1;&#x7406;&#x8005;</p>
        <p>&#x30EA;&#x30B9;&#x30C8;&#x5024;&#x8868;&#x793A;</p>
      </td>
    </tr>
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
      <td style="text-align:left">&#x30E1;&#x30FC;&#x30EB;&#x3000;&#x3000;&#x914D;&#x4FE1;</td>
      <td style="text-align:left">
        <p>&#x30FB;&#x62BC;&#x4E0B;&#x3067;&#x56FA;&#x5B9A;&#x6587;&#x8A00;&#x306E;&#x30E1;&#x30FC;&#x30EB;&#x3092;&#x6307;&#x5B9A;&#x3057;&#x305F;&#x30E6;&#x30FC;&#x30B6;&#x306E;&#x30E1;&#x30FC;&#x30EB;&#x30A2;&#x30C9;&#x30EC;&#x30B9;&#x306B;&#x9001;&#x4FE1;&#x3059;&#x308B;</p>
        <p>&#x30FB;API&#x30B5;&#x30FC;&#x30D0;&#x3067;&#x9001;&#x4FE1;&#x5148;&#x3084;&#x984C;&#x540D;&#x3001;&#x672C;&#x6587;&#x3092;&#x30BB;&#x30C3;&#x30C8;&#x3057;&#x3001;&#x5225;&#x30D1;&#x30C3;&#x30B1;&#x30FC;&#x30B8;&#x304B;&#x3089;SendGrid&#x3068;&#x9023;&#x643A;&#x3092;&#x3059;&#x308B;</p>
        <p>&#x30FB;SendGrid&#x60C5;&#x5831;&#x306A;&#x3069;&#x306F;env&#x8A2D;&#x5B9A;</p>
      </td>
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
| 8 | ID | 表示 | textlink |
| 9 | メールアドレス | 表示 | text |
| 10 | 権限 | 表示 | text |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 8 | ID | 押下でS102\_3 ユーザー編集画面に遷移 |
| 10 | 権限 | リスト値=1:システム管理者 表示 |
{% endtab %}

{% tab title="表示API" %}
**使用API**

**usersearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 8 | ID | userId |
| 9 | メールアドレス | email |
| 10 | 権限 | userFlag |
{% endtab %}
{% endtabs %}

