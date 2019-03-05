# S105\_2 請求先編集

### 請求先情報部

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
      <th style="text-align:left">&#x5FC5;&#x9808;</th>
      <th style="text-align:left">&#x6587;&#x5B57;&#x6570;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x5148;&#x540D;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x3075;&#x308A;&#x304C;&#x306A;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x5148;&#x62C5;&#x5F53;&#x8005;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x90F5;&#x4FBF;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">8</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">&#x90FD;&#x9053;&#x5E9C;&#x770C;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x4F4F;&#x6240;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">300</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x7121;&#x52B9;&#x30D5;&#x30E9;&#x30B0;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">check</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**billingSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | billingId |

#### セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | billingId |
| 2 | 顧客名 | customerName |
| 3 | 請求先名 | name |
| 4 | ふりがな | kana |
| 5 | 請求先担当者 | staffName |
| 6 | 郵便番号 | zip |
| 7 | 都道府県 | address1 |
| 8 | 住所 | address2 |
| 9 | 無効フラグ | disableFlag |
{% endtab %}

{% tab title="詳細仕様" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">&#x8868;&#x793A;&#x6761;&#x4EF6;/</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">customerId&#x304B;&#x3089;[customerId - customerName]&#x3092;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x3075;&#x308A;&#x304C;&#x306A;</td>
      <td style="text-align:left">&#x3072;&#x3089;&#x304C;&#x306A;&#x306E;&#x307F;&#x4FDD;&#x5B58;&#x53EF;&#x80FD;</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x90F5;&#x4FBF;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x6570;&#x5024;&#x306E;&#x307F;&#x4FDD;&#x5B58;&#x53EF;&#x80FD;</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x90F5;&#x4FBF;&#x756A;&#x53F7;</td>
      <td style="text-align:left">xxx-xxxx &#x3068;&#x3044;&#x3046;&#x5F62;&#x306E;&#x307F;&#x8A31;&#x5BB9;</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">&#x90FD;&#x9053;&#x5E9C;&#x770C;</td>
      <td style="text-align:left">
        <p>&#x5165;&#x529B;&#x3057;&#x305F;&#x90F5;&#x4FBF;&#x756A;&#x53F7;&#x304B;&#x3089;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x4E0D;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x4F4F;&#x6240;</td>
      <td style="text-align:left">
        <p>&#x5165;&#x529B;&#x3057;&#x305F;&#x90F5;&#x4FBF;&#x756A;&#x53F7;&#x304B;&#x3089;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S105_2
          &#x8ACB;&#x6C42;&#x5148;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

billingSave

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | billingId |
| 2 | 顧客名 | customerId |
| 3 | 請求先名 | name |
| 4 | ふりがな | kana |
| 5 | 請求先担当者 | staffName |
| 6 | 郵便番号 | zip |
| 7 | 都道府県 | address1 |
| 8 | 住所 | address2 |
| 9 | 無効フラグ | disableFlag |
{% endtab %}

{% tab title="その他API" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">&#x540D;&#x79F0;</th>
      <th style="text-align:left">&#x30BF;&#x30A4;&#x30DF;&#x30F3;&#x30B0;</th>
      <th style="text-align:left">API</th>
      <th style="text-align:left">&#x5185;&#x5BB9;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x90F5;&#x4FBF;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;&#x6642;</td>
      <td style="text-align:left">addressSearch</td>
      <td style="text-align:left">
        <p>&#x5165;&#x529B;&#x3057;&#x305F;&#x90F5;&#x4FBF;&#x756A;&#x53F7;&#x3092;[zipCode]&#x306B;&#x30BB;&#x30C3;&#x30C8;&#x3059;&#x308B;</p>
        <p>&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;&#x60C5;&#x5831;&#x3092;&#x5143;&#x306B;[&#x90FD;&#x9053;&#x5E9C;&#x770C;][&#x4F4F;&#x6240;]&#x9805;&#x76EE;&#x3092;&#x66F4;&#x65B0;&#x3059;&#x308B;</p>
        <p>&#x691C;&#x7D22;&#x7D50;&#x679C;&#x304C;0&#x4EF6;&#x306E;&#x5834;&#x5408;&#x3001;&#x30D0;&#x30EA;&#x30C7;&#x30FC;&#x30B7;&#x30E7;&#x30F3;NG</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

