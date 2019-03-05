# S113\_3 担当者編集

### 担当者情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ID | 表示 | text | Y |  |
| 2 | 担当者名 | 更新 | text | Y | 50 |
| 3 | 担当部署ID検索 | 表示 | button | Y |  |
| 4 | 担当部署 | 更新 | text | Y |  |
| 5 | 在籍区分 | 更新 | list |  |  |
| 6 | 保存 | 表示 | button |  |  |
| 7 | 戻る | 表示 | button |  |  |
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

#### staffSerch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | staffId |

#### セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | staffId |
| 2 | 担当者名 | staffName |
| 4 | 担当部署 | sectionId |
| 5 | 在籍区分 | type |
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
      <td style="text-align:left">3</td>
      <td style="text-align:left">&#x62C5;&#x5F53;&#x8005;ID&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>&#x5E38;&#x306B;&#x8868;&#x793A;</p>
        <p>&#x62BC;&#x4E0B;&#x3067;S112_1 &#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x4E00;&#x89A7;&#x753B;&#x9762;POPUP&#x8868;&#x793A;</p>
        <p>ID&#x62BC;&#x4E0B;&#x3067;&#x5F53;&#x753B;&#x9762;&#x9077;&#x79FB;&#x3001;&#x62C5;&#x5F53;&#x90E8;&#x7F72;ID&#x3001;&#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x540D;</p>
        <p>&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x62C5;&#x5F53;&#x90E8;&#x7F72;</td>
      <td style="text-align:left">
        <p>&#x8D77;&#x52D5;&#x6642;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x306E;sectionId&#x304B;&#x3089;[sectionId
          - sectionName]&#x3092;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x5728;&#x7C4D;&#x533A;&#x5206;</td>
      <td style="text-align:left">
        <p>1.&#x5728;&#x7C4D; 2.&#x4F11;&#x8077; 3.&#x9000;&#x8077;</p>
        <p>&#x30EA;&#x30B9;&#x30C8;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S113_3
          &#x62C5;&#x5F53;&#x8005;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

#### staffSave

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | staffId |
| 2 | 担当者名 | staffName |
| 4 | 担当部署 | sectionId |
| 5 | 在籍区分 | type |
{% endtab %}
{% endtabs %}

