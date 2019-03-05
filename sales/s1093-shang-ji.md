# S109\_3 売上編集

### **売上情報部**

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ID | 表示 | text | Y |  |
| 2 | 顧客名 | 更新 | text | Y | 100 |
| 3 | ふりがな | 更新 | text |  | 200 |
| 4 | 電話番号 | 更新 | text |  | 100 |
| 5 | 担当者 | 更新 | text |  | 50 |
| 6 | メールアドレス | 更新 | text |  | 100 |
| 7 | 郵便番号 | 更新 | text |  | 8 |
| 8 | 都道府県 | 表示 | text |  |  |
| 9 | 住所 | 更新 | text |  | 300 |
| 10 | 納品先 | 更新 | list |  |  |
| 11 | 請求先 | 更新 | list |  |  |
| 12 | 請求日 | 更新 | date |  |  |
| 13 | 支払期限日 | 更新 | date |  |  |
| 14 | 区分 | 更新 | list |  |  |
{% endtab %}

{% tab title="起動時API" %}
#### 使用API① <a id="shi-yong-api"></a>

**salesDetailSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |

**セット内容（売上明細は売上明細部に記載）**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billingId |
| 12 | 請求日 | billingDate |
| 13 | 支払期限日 | paymentDate |
| 14 | 区分 | type |
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
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">customerId&#x304B;&#x3089;[customerId - name]&#x3092;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x90FD;&#x9053;&#x5E9C;&#x770C;</td>
      <td style="text-align:left">
        <p>&#x5165;&#x529B;&#x3057;&#x305F;&#x90F5;&#x4FBF;&#x756A;&#x53F7;&#x304B;&#x3089;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x4E0D;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x4F4F;&#x6240;</td>
      <td style="text-align:left">
        <p>&#x5165;&#x529B;&#x3057;&#x305F;&#x90F5;&#x4FBF;&#x756A;&#x53F7;&#x304B;&#x3089;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x7D0D;&#x54C1;&#x5148;</td>
      <td style="text-align:left">
        <p>&#x753B;&#x9762;&#x8D77;&#x52D5;&#x6642;&#x306B;&#x7D0D;&#x54C1;&#x5148;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x8FD4;&#x5374;&#x5024;&#x306B;&#x73FE;&#x5728;&#x306E;locationId&#x304C;&#x5B58;&#x5728;&#x3059;&#x308B;&#x5834;&#x5408;&#x306F;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x30BB;&#x30C3;&#x30C8;</p>
        <p>&#x5B58;&#x5728;&#x3057;&#x306A;&#x3044;&#x5834;&#x5408;&#x306F;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x7121;&#x3057;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x5148;</td>
      <td style="text-align:left">
        <p>&#x753B;&#x9762;&#x8D77;&#x52D5;&#x6642;&#x306B;&#x8ACB;&#x6C42;&#x5148;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x8FD4;&#x5374;&#x5024;&#x306B;&#x73FE;&#x5728;&#x306E;locationId&#x304C;&#x5B58;&#x5728;&#x3059;&#x308B;&#x5834;&#x5408;&#x306F;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x30BB;&#x30C3;&#x30C8;</p>
        <p>&#x5B58;&#x5728;&#x3057;&#x306A;&#x3044;&#x5834;&#x5408;&#x306F;&#x30C7;&#x30D5;&#x30A9;&#x30EB;&#x30C8;&#x7121;&#x3057;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">&#x533A;&#x5206;</td>
      <td style="text-align:left">
        <p>-</p>
        <p>1.&#x53D7;&#x8A17;</p>
        <p>2.SES &#x30EA;&#x30B9;&#x30C8;&#x5024;&#x8868;&#x793A;</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="納品先API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**locationSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
{% endtab %}

{% tab title="請求先API" %}
#### 使用API <a id="shi-yong-api-2"></a>

**billingSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
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
      <td style="text-align:left">7</td>
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

### 売上明細ヘッダー部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 15 | 明細追加 | 表示 | button |
| 16 | 明細削除 | 表示 | button |
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
      <td style="text-align:left">15</td>
      <td style="text-align:left">&#x660E;&#x7D30;&#x8FFD;&#x52A0;</td>
      <td style="text-align:left">&#x898B;&#x7A4D;&#x660E;&#x7D30;&#x90E8;&#x3001;&#x4E00;&#x756A;&#x4E0B;&#x306B;1&#x884C;&#x660E;&#x7D30;&#x3092;&#x8FFD;&#x52A0;&#x3059;&#x308B;</td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">&#x660E;&#x7D30;&#x524A;&#x9664;</td>
      <td style="text-align:left">
        <p>&#x78BA;&#x8A8D;&#x30C0;&#x30A4;&#x30A2;&#x30ED;&#x30B0;&#x3092;&#x8868;&#x793A;&#x3057;&#x3001;&#x898B;&#x7A4D;&#x660E;&#x7D30;&#x90E8;&#x3001;&#x30C1;&#x30A7;&#x30C3;&#x30AF;
          = ON</p>
        <p>&#x306E;&#x884C;&#x3092;&#x524A;&#x9664;&#x3059;&#x308B;</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

### 売上明細部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 文字数 |
| :--- | :--- | :--- | :--- | :--- |
| 17 | チェック | 更新 | check |  |
| 18 | No | 表示 | text |  |
| 19 | 題名 | 更新 | text | 200 |
| 20 | 詳細 | 更新 | text | 300 |
| 21 | 単価 | 更新 | text |  |
| 22 | 数量 | 更新 | text |  |
| 23 | 金額 | 表示 | text |  |
{% endtab %}

{% tab title="起動時API" %}
**使用APIは売上情報部に記載済み**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | title |
| 20 | 詳細 | detail |
| 21 | 単価 | unitPrice |
| 22 | 数量 | count |
| 23 | 金額 | amount |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 18 | No | 画面上の連番 |
| 23 | 金額 | 単価 \* 数量 |
{% endtab %}
{% endtabs %}

### 売上明細フッダー部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 24 | 税抜金額 | 表示 | text |
| 25 | 消費税率 | 表示 | hidden |
| 26 | 消費税額 | 表示 | text |
| 27 | 税込金額 | 表示 | text |
{% endtab %}

{% tab title="起動時API" %}
**使用APIは売上情報部に記載済み**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 24 | 税抜金額 | amount |
| 25 | 消費税率 | taxRate |
| 26 | 消費税額 | tax |
| 27 | 税込金額 | totalAmount |
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
      <td style="text-align:left">24</td>
      <td style="text-align:left">&#x7A0E;&#x629C;&#x91D1;&#x984D;</td>
      <td style="text-align:left">&#x58F2;&#x4E0A;&#x660E;&#x7D30;&#x90E8;&#x3001;&#x91D1;&#x984D;&#x306E;&#x5408;&#x8A08;&#x5024;</td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">&#x6D88;&#x8CBB;&#x7A0E;&#x7387;</td>
      <td style="text-align:left">&#x753B;&#x9762;&#x4E0A;&#x975E;&#x8868;&#x793A;&#x3001;&#x767B;&#x9332;&#x6642;&#x306E;&#x5024;&#x3092;&#x4F7F;&#x7528;&#x3001;&#x5909;&#x66F4;&#x4E0D;&#x53EF;&#x3067;&#x5909;&#x308F;&#x308B;&#x3053;&#x3068;&#x306F;&#x306A;&#x3057;</td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
      <td style="text-align:left">&#x6D88;&#x8CBB;&#x7A0E;&#x984D;</td>
      <td style="text-align:left">
        <p>&#x7A0E;&#x629C;&#x91D1;&#x984D; * &#x6D88;&#x8CBB;&#x7A0E;&#x7387;</p>
        <p>&#x5C0F;&#x6570;&#x70B9;&#x4EE5;&#x4E0B;&#x306E;&#x5024;&#x56DB;&#x6368;&#x4E94;&#x5165;&#x3057;&#x3066;&#x6574;&#x6570;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">&#x7A0E;&#x8FBC;&#x91D1;&#x984D;</td>
      <td style="text-align:left">
        <p>&#x7A0E;&#x629C;&#x91D1;&#x984D; + &#x6D88;&#x8CBB;&#x7A0E;&#x984D;</p>
        <p>&#x5C0F;&#x6570;&#x70B9;&#x4EE5;&#x4E0B;&#x306E;&#x5024;&#x56DB;&#x6368;&#x4E94;&#x5165;&#x3057;&#x3066;&#x6574;&#x6570;&#x8868;&#x793A;</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 24 | 保存 | 表示 | button |
| 25 | 戻る | 表示 | button |
| 26 | エクセル出力ボタン | 表示 | button |
| 27 | PDF出力ボタン | 表示 | button |
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
      <td style="text-align:left">24</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S109_3
          &#x58F2;&#x4E0A;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
      <td style="text-align:left">&#x30A8;&#x30AF;&#x30BB;&#x30EB;&#x51FA;&#x529B;&#x3000;&#x3000;&#x3000;&#x3000;&#x3000;&#x3000;&#x30DC;&#x30BF;&#x30F3;</td>
      <td
      style="text-align:left">&#x62BC;&#x4E0B;&#x3067;&#x58F2;&#x4E0A;&#x3001;&#x58F2;&#x4E0A;&#x660E;&#x7D30;&#x60C5;&#x5831;&#x30A8;&#x30AF;&#x30BB;&#x30EB;&#x51FA;&#x529B;</td>
    </tr>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">PDF&#x51FA;&#x529B;&#x30DC;&#x30BF;&#x30F3;</td>
      <td style="text-align:left">&#x62BC;&#x4E0B;&#x3067;&#x58F2;&#x4E0A;&#x3001;&#x58F2;&#x4E0A;&#x660E;&#x7D30;&#x60C5;&#x5831;PDF&#x51FA;&#x529B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API <a id="shi-yong-api-3"></a>

**salesSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billinbId |
| 12 | 請求日 | billingDate |
| 13 | 支払期限日 | paymentDate |
| 24 | 税抜合計 | amount |
| 25 | 消費税率 | taxRate |
| 26 | 消費税額 | tax |
| 27 | 税込金額 | totalAmount |
| 14 | 区分 | types |
| - | 売上明細数 | detailCount |

**売上明細（売上 1 に対して 売上明細 N）**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | title |
| 20 | 詳細 | detail |
| 21 | 単価 | unitPrice |
| 22 | 数量 | count |
| 23 | 金額 | amount |
{% endtab %}
{% endtabs %}

