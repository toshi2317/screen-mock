# S110\_2 クレーム登録

### **クレーム情報部**

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 顧客検索 | 表示 | button | Y |  |
| 2 | 顧客名 | 表示 | text | Y |  |
| 3 | 受注ID検索ボタン | 表示 | button | Y |  |
| 4 | 受注ID | 表示 | text |  |  |
| 5 | 題名 | 更新 | text |  | 200 |
| 6 | 内容 | 更新 | textarea |  | 1000 |
| 7 | 保存 | 表示 | button |  |  |
| 8 | 戻る | 表示 | button |  |  |
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
      <td style="text-align:left">1</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>GET&#x30D1;&#x30E9;&#x30E1;&#x30FC;&#x30BF;&#x306B;customerId&#x304C;&#x5B58;&#x5728;&#x3059;&#x308B;&#x5834;&#x5408;&#x3001;
          &#x9867;&#x5BA2;API&#x3001;&#x53D7;&#x6CE8;&#x5148;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x5F53;&#x30DC;&#x30BF;&#x30F3;&#x975E;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x691C;&#x7D22;</td>
      <td style="text-align:left">
        <p>GET&#x30D1;&#x30E9;&#x30E1;&#x30FC;&#x30BF;&#x306B;customerId&#x304C;&#x5B58;&#x5728;&#x3057;&#x306A;&#x3044;&#x5834;&#x5408;</p>
        <p>&#x9867;&#x5BA2;&#x691C;&#x7D22;&#x30DC;&#x30BF;&#x30F3;&#x3092;&#x8868;&#x793A;&#x3057;&#x3001;&#x62BC;&#x4E0B;&#x3067;S103_1
          &#x9867;&#x5BA2;&#x4E00;&#x89A7;&#x3092;POPUP&#x8868;&#x793A;</p>
        <p>&#x5F53;&#x753B;&#x9762;&#x306B;&#x623B;&#x3063;&#x3066;&#x304D;&#x305F;&#x969B;&#x3001;&#x9867;&#x5BA2;API&#x3092;&#x5B9F;&#x884C;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">&#x9867;&#x5BA2;&#x540D;</td>
      <td style="text-align:left">&#x9078;&#x629E;&#x3055;&#x308C;&#x3066;&#x3044;&#x308B;&#x9867;&#x5BA2;&#x306E;[customerId
        - name]&#x3092;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">
        <p>&#x53D7;&#x6CE8;ID</p>
        <p>&#x691C;&#x7D22;</p>
        <p>&#x30DC;&#x30BF;&#x30F3;</p>
      </td>
      <td style="text-align:left">
        <p>&#x9867;&#x5BA2;&#x9078;&#x629E;&#x3055;&#x308C;&#x305F;&#x6642;&#x70B9;&#x3067;&#x8868;&#x793A;</p>
        <p>&#x53D7;&#x6CE8;ID&#x691C;&#x7D22;&#x30DC;&#x30BF;&#x30F3;&#x62BC;&#x4E0B;&#x3067;S108_1&#x53D7;&#x6CE8;&#x4E00;&#x89A7;&#x753B;&#x9762;&#x9078;&#x629E;&#x3055;&#x308C;&#x305F;&#x9867;&#x5BA2;&#x306E;&#x53D7;&#x6CE8;&#x60C5;&#x5831;POPUP&#x8868;&#x793A;</p>
        <p>ID&#x62BC;&#x4E0B;&#x3067;&#x5F53;&#x753B;&#x9762;&#x9077;&#x79FB;&#x3001;&#x53D7;&#x6CE8;ID&#x81EA;&#x52D5;&#x63D0;&#x6848;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S110_3
          &#x30AF;&#x30EC;&#x30FC;&#x30E0;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
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
#### 使用API <a id="shi-yong-api"></a>

**claimSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 3 | 受注ID | orderId |
| 4 | 題名 | title |
| 5 | 内容 | contents  |
{% endtab %}

{% tab title="顧客API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**customerSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
{% endtab %}
{% endtabs %}

