# S108\_3 受注編集

### **受注情報部**

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
| 8 | 都道府県 | 表示 | text |  | 50 |
| 9 | 住所 | 更新 | text |  | 300 |
|  | 担当部署検索ボタン | 表示 | button | Y |  |
|  | 担当部署 | 表示 | text |  | 100 |
|  | 部署担当者 | 更新 | list |  | 50 |
| 10 | 納品先 | 更新 | list |  |  |
| 11 | 請求先 | 更新 | list |  |  |
| 12 | 見積ID | 表示 | text |  |  |
| 13 | 受注日 | 更新 | date |  |  |
| 14 | 納品日 | 更新 | date |  |  |
| 15 | 契約金額 | 更新 | text |  |  |
| 16 | 区分 | 更新 | list |  |  |
| 17 | 保存 | 表示 | button |  |  |
| 18 | 戻る | 表示 | button |  |  |
{% endtab %}

{% tab title="起動時API" %}
**使用API**

orderSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | orderId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | orderId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
|  | 担当部署 | sectionId |
|  | 部署担当者 | staffId |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billingId |
| 12 | 見積先 | quotationId |
| 13 | 受注日 | orderDate |
| 14 | 納品日 | deliveryDate |
| 15 | 契約金額 | contractAmount |
| 16 | 区分 | type |
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
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x691C;&#x7D22;&#x30DC;&#x30BF;&#x30F3;</td>
      <td
      style="text-align:left">
        <p>&#x62BC;&#x4E0B;&#x3067;S112_1 &#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x4E00;&#x89A7;&#x3092;POPUP&#x8868;&#x793A;</p>
        <p>&#x5F53;&#x753B;&#x9762;&#x306B;&#x623B;&#x3063;&#x3066;&#x304D;&#x305F;&#x969B;&#x3001;&#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x540D;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x62C5;&#x5F53;&#x90E8;&#x7F72;</td>
      <td style="text-align:left">
        <p>&#x8D77;&#x52D5;&#x6642;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x81EA;&#x52D5;&#x63D0;&#x6848;
          or</p>
        <p>S112_1 &#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x4E00;&#x89A7;&#x753B;&#x9762;&#x3067;&#x9078;&#x629E;&#x3055;&#x308C;&#x305F;</p>
        <p>[sectionId - sectionName]&#x3092;&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
        <p>&#x5909;&#x66F4;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">&#x90E8;&#x7F72;&#x62C5;&#x5F53;&#x8005;</td>
      <td style="text-align:left">
        <p>&#x8D77;&#x52D5;&#x6642;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x81EA;&#x52D5;&#x63D0;&#x6848;
          or &#x62C5;&#x5F53;&#x90E8;&#x7F72;&#x9078;&#x629E;&#x3067;&#x62C5;&#x5F53;&#x8005;API&#x5B9F;&#x884C;</p>
        <p>&#x62C5;&#x5F53;&#x8005;API&#x306E;&#x7D50;&#x679C;[staffId - staffName]&#x3092;&#x30EA;&#x30B9;&#x30C8;&#x8868;&#x793A;</p>
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
      <td style="text-align:left">12</td>
      <td style="text-align:left">&#x898B;&#x7A4D;ID</td>
      <td style="text-align:left">
        <p>&#x898B;&#x7A4D;ID = NULL&#x306E;&#x5834;&#x5408;&#x306F;&#x5F53;&#x9805;&#x76EE;&#x975E;&#x8868;&#x793A;</p>
        <p>&#x5909;&#x66F4;&#x4E0D;&#x53EF;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">&#x533A;&#x5206;</td>
      <td style="text-align:left">
        <p>-</p>
        <p>1.&#x53D7;&#x8A17;</p>
        <p>2.SES &#x30EA;&#x30B9;&#x30C8;&#x5024;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x4FDD;&#x5B58;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S108_3
          &#x53D7;&#x6CE8;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="担当者API" %}
**使用API**

**staffSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
|  | 担当部署 | sectionId |
{% endtab %}

{% tab title="納品先API" %}
**使用API**

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
      <th style="text-align:left"><b>No</b>
      </th>
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

{% tab title="保存API" %}
**使用API**

**orderSave**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | orderId |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
|  | 担当部署 | sectionId |
|  | 部署担当者 | staffId |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billinbId |
| 12 | 見積ID | quotationId |
| 13 | 受注日 | orderDate |
| 14 | 納品日 | deliveryDate |
| 15 | 契約金額 | contractAmount |
| 16 | 区分 | types |
{% endtab %}
{% endtabs %}

### **売上情報ボタン部**

{% tabs %}
{% tab title="項目制御" %}
| **No** | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 19 | 新規登録 | 表示 | button |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 19 | 新規登録 | 押下でS109\_2登録画面へ遷移 |
| 19 | 新規登録 | 遷移時、orderIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### **売上情報一覧部**

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 20 | ID | 表示 | textlink |
| 21 | 請求日 | 表示 | text |
| 22 | 支払期限日 | 表示 | text |
| 23 | 税込金額 | 表示 | text |
| 24 | 区分 | 表示 | text |
{% endtab %}

{% tab title="起動時API" %}
**使用API**

salesSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | orderId |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 20 | ID | 押下でS109\_3 売上編集画面を別タブ起動 |
{% endtab %}

{% tab title="表示パラメータ名" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 20 | ID | salesId |
| 21 | 請求日 | billingDate |
| 22 | 支払期限日 | paymentDate |
| 23 | 税込金額 | amount |
| 24 | 区分 | types |
{% endtab %}
{% endtabs %}

