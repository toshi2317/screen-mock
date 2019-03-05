# S114\_1 ファイル出力状況一覧

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | ID | 更新 | text |
| 2 | ステータス | 更新 | list |
| 3 | 出力依頼日\(From\) | 更新 | date |
| 4 | 出力依頼日\(To\) | 更新 | date |
| 5 | クリア | 表示 | button |
| 6 | 検索 | 表示 | button |
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
      <td style="text-align:left">2</td>
      <td style="text-align:left">&#x30B9;&#x30C6;&#x30FC;&#x30BF;&#x30B9;</td>
      <td style="text-align:left">
        <p>--</p>
        <p>1.&#x5F85;&#x6A5F;&#x4E2D;</p>
        <p>2.&#x5B9F;&#x884C;&#x4E2D;</p>
        <p>3.&#x5B8C;&#x4E86;</p>
        <p>9.&#x5931;&#x6557;</p>
        <p>&#x30EA;&#x30B9;&#x30C8;&#x5024;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">&#x51FA;&#x529B;&#x4F9D;&#x983C;&#x65E5;(From)</td>
      <td style="text-align:left">&#x5F53;&#x65E5;&#x3092;&#x81EA;&#x52D5;&#x63D0;&#x6848;</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x30AF;&#x30EA;&#x30A2;</td>
      <td style="text-align:left">&#x691C;&#x7D22;&#x6761;&#x4EF6;&#x90E8;&#x3092;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x306E;&#x72B6;&#x614B;&#x306B;&#x623B;&#x3059;</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>&#x691C;&#x7D22;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x691C;&#x7D22;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x3092;&#x4E00;&#x89A7;&#x8868;&#x793A;&#x90E8;&#x306B;&#x8868;&#x793A;&#x3059;&#x308B;</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
**使用API**

**fileStatusSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | fileStatusId |
| 2 | ステータス | status |
| 3 | 出力依頼日\(From\) | createdAtFrom |
| 4 | 出力依頼日\(To\) | createdAtTo |
{% endtab %}
{% endtabs %}

### 一覧情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 5 | ID | 表示 | text |
| 6 | SQSキューID | 表示 | text |
| 7 | S3ファイルパス | 表示 | textlink |
| 8 | ステータス | 表示 | text |
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
      <td style="text-align:left">7</td>
      <td style="text-align:left">S3&#x30D5;&#x30A1;&#x30A4;&#x30EB;</td>
      <td style="text-align:left">&#x62BC;&#x4E0B;&#x3067;CSV&#x30D5;&#x30A1;&#x30A4;&#x30EB;&#x51FA;&#x529B;</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x30B9;&#x30C6;&#x30FC;&#x30BF;&#x30B9;</td>
      <td style="text-align:left">
        <p>1.&#x5F85;&#x6A5F;&#x4E2D; 2.&#x5B9F;&#x884C;&#x4E2D; 3.&#x5B8C;&#x4E86;
          9.&#x5931;&#x6557;</p>
        <p>&#x30B9;&#x30C6;&#x30FC;&#x30BF;&#x30B9;&#x306E;&#x5024;&#x306E;&#x6587;&#x8A00;&#x8868;&#x793A;</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
**使用API**

**fileStatusSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 5 | ID | fileStatusId |
| 6 | SQSキューID | sqsId |
| 7 | S3ファイル | filePath |
| 8 | ステータス | status |
{% endtab %}
{% endtabs %}

