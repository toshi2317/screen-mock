# S109\_2 売上登録

### **売上情報部**

{% tabs %}
{% tab title="項目制御" %}


| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 顧客名 | 更新 | text | Y | 100 |
| 2 | ふりがな | 更新 | text |  | 200 |
| 3 | 電話番号 | 更新 | text |  | 100 |
| 4 | 担当者 | 更新 | text |  | 50 |
| 5 | メールアドレス | 更新 | text |  | 100 |
| 6 | 郵便番号 | 更新 | text |  | 8 |
| 7 | 都道府県 | 表示 | text |  |  |
| 8 | 住所 | 更新 | text |  | 300 |
| 9 | 納品先 | 更新 | list |  |  |
| 10 | 請求先 | 更新 | list |  |  |
| 11 | 請求日 | 更新 | date |  |  |
| 12 | 支払期限日 | 更新 | date |  |  |
| 13 | 区分 | 更新 | list |  |  |
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
      <td style="text-align:left">-</td>
      <td style="text-align:left">&#x8D77;&#x52D5;&#x6642;API</td>
      <td style="text-align:left">
        <p>GET&#x30D1;&#x30E9;&#x30E1;&#x30FC;&#x30BF;&#x306E;orderId&#x304B;&#x3089;API&#x53E9;&#x304B;&#x308C;&#x3066;&#x8FD4;&#x5374;&#x5024;</p>
        <p>&#x81EA;&#x52D5;&#x63D0;&#x6848;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">customerId&#x304B;&#x3089;[customerId - name]&#x3092;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">&#x3075;&#x308A;&#x304C;&#x306A;</td>
      <td style="text-align:left">&#x3072;&#x3089;&#x304C;&#x306A;&#x306E;&#x307F;&#x4FDD;&#x5B58;&#x53EF;&#x80FD;</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">&#x96FB;&#x8A71;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x6570;&#x5024;&#x306E;&#x307F;&#x4FDD;&#x5B58;&#x53EF;&#x80FD;</td>
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
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x7D0D;&#x54C1;&#x5148;</td>
      <td style="text-align:left">&#x7D0D;&#x54C1;&#x5148;API&#x306E;&#x7D50;&#x679C;[locationId - name]&#x3092;&#x30EA;&#x30B9;&#x30C8;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x5148;</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x5148;API&#x306E;&#x7D50;&#x679C;[billingId - name]&#x3092;&#x30EA;&#x30B9;&#x30C8;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">&#x8ACB;&#x6C42;&#x65E5;</td>
      <td style="text-align:left">&#x5F53;&#x65E5;&#x3092;&#x81EA;&#x52D5;&#x63D0;&#x6848;</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">&#x652F;&#x6255;&#x671F;&#x9650;&#x65E5;</td>
      <td style="text-align:left">&#x5F53;&#x65E5; + 1&#x30F6;&#x6708;&#x306E;&#x6708;&#x672B;&#x65E5;&#x3092;&#x81EA;&#x52D5;&#x63D0;&#x6848;</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
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

{% tab title="起動時API" %}
#### 使用API

**orderSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| - | 受注ID | orderId |

#### セット内容

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
| 1 | 顧客名 | customerName |
| 2 | ふりがな | customerKana |
| 3 | 電話番号 | customerTel |
| 4 | 担当者 | customerStaffName |
| 5 | メールアドレス | customerEmail |
| 6 | 郵便番号 | customerZip |
| 7 | 都道府県 | customerAddress1 |
| 8 | 住所 | customerAddress2 |
| 9 | 納品先 | locationId |
| 10 | 請求先 | billinbId |
{% endtab %}

{% tab title="納品先API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**locationSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
{% endtab %}

{% tab title="請求先API" %}
#### 使用API <a id="shi-yong-api-2"></a>

**billingSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
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

### 売上明細ヘッダー部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 14 | 明細追加 | 表示 | button |
| 15 | 明細削除 | 表示 | button |
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
      <td style="text-align:left">14</td>
      <td style="text-align:left">&#x660E;&#x7D30;&#x8FFD;&#x52A0;</td>
      <td style="text-align:left">&#x898B;&#x7A4D;&#x660E;&#x7D30;&#x90E8;&#x3001;&#x4E00;&#x756A;&#x4E0B;&#x306B;1&#x884C;&#x660E;&#x7D30;&#x3092;&#x8FFD;&#x52A0;&#x3059;&#x308B;</td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
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
| 16 | チェック | 更新 | check |  |
| 17 | No | 表示 | text |  |
| 18 | 題名 | 更新 | text | 200 |
| 19 | 詳細 | 更新 | text | 300 |
| 20 | 単価 | 更新 | text |  |
| 21 | 数量 | 更新 | text |  |
| 22 | 金額 | 表示 | text |  |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 17 | No | 画面上の連番 |
| 22 | 金額 | 単価 \* 数量 |
{% endtab %}
{% endtabs %}

### 売上明細フッダー部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 23 | 税抜金額 | 表示 | text |
| 24 | 消費税率 | 表示 | hidden |
| 25 | 消費税額 | 表示 | text |
| 26 | 税込金額 | 表示 | text |
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
      <td style="text-align:left">23</td>
      <td style="text-align:left">&#x7A0E;&#x629C;&#x91D1;&#x984D;</td>
      <td style="text-align:left">&#x58F2;&#x4E0A;&#x660E;&#x7D30;&#x90E8;&#x3001;&#x91D1;&#x984D;&#x306E;&#x5408;&#x8A08;&#x5024;</td>
    </tr>
    <tr>
      <td style="text-align:left">24</td>
      <td style="text-align:left">&#x6D88;&#x8CBB;&#x7A0E;&#x7387;</td>
      <td style="text-align:left">
        <p>&#x753B;&#x9762;&#x4E0A;&#x975E;&#x8868;&#x793A;&#x3001;&#x6D88;&#x8CBB;&#x7A0E;&#x7387;&#x306E;&#x53D6;&#x5F97;&#x65B9;&#x6CD5;&#x306F;&#x6D88;&#x8CBB;&#x7A0E;&#x7387;&#x691C;&#x7D22;API&#x53C2;&#x7167;</p>
        <p>&#x8ACB;&#x6C42;&#x65E5;&#x3092;&#x5143;&#x306B;tax_rate&#x3092;&#x53D6;&#x5F97;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">&#x6D88;&#x8CBB;&#x7A0E;&#x984D;</td>
      <td style="text-align:left">
        <p>&#x7A0E;&#x629C;&#x91D1;&#x984D; * &#x6D88;&#x8CBB;&#x7A0E;&#x7387;</p>
        <p>&#x5C0F;&#x6570;&#x70B9;&#x4EE5;&#x4E0B;&#x306E;&#x5024;&#x56DB;&#x6368;&#x4E94;&#x5165;&#x3057;&#x3066;&#x6574;&#x6570;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
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
| 27 | 保存 | 表示 | button |
| 28 | 戻る | 表示 | button |
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
      <td style="text-align:left">27</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S109_3
          &#x58F2;&#x4E0A;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">28</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API <a id="shi-yong-api-3"></a>

**salesSave**

**売上**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
| 1 | 顧客名 | customerName |
| 2 | ふりがな | customerKana |
| 3 | 電話番号 | customerTel |
| 4 | 担当者 | customerStaffName |
| 5 | メールアドレス | customerEmail |
| 6 | 郵便番号 | customerZip |
| 7 | 都道府県 | customerAddress1 |
| 8 | 住所 | customerAddress2 |
| 9 | 納品先 | locationId |
| 10 | 請求先 | billinbId |
| 11 | 請求日 | billingDate |
| 12 | 支払期限日 | paymentDate |
| 23 | 税抜合計 | amount |
| 24 | 消費税率 | taxRate |
| 25 | 消費税額 | tax |
| 26 | 税込金額 | totalAmount |
| 13 | 区分 | types |
| - | 売上明細数 | detailCount |

**売上明細（売上 1 に対して 売上明細 N）**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | detailTitle |
| 20 | 詳細 | detailDetail |
| 21 | 単価 | detailUnitPrice |
| 22 | 数量 | detailCount |
| 23 | 金額 | detailAmount |
{% endtab %}
{% endtabs %}

