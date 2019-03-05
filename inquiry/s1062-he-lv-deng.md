# S106\_2 問合履歴登録

### 問合履歴情報部

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
      <td style="text-align:left">&#x9867;&#x5BA2;&#x691C;&#x7D22;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">button</td>
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
      <td style="text-align:left">&#x554F;&#x5408;&#x62C5;&#x5F53;&#x8005;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x96FB;&#x8A71;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x30E1;&#x30FC;&#x30EB;&#x30A2;&#x30C9;&#x30EC;&#x30B9;</td>
      <td
      style="text-align:left">&#x66F4;&#x65B0;</td>
        <td style="text-align:left">text</td>
        <td style="text-align:left"></td>
        <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x984C;&#x540D;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x5185;&#x5BB9;</td>
      <td style="text-align:left">&#x66F4;&#x65B0;</td>
      <td style="text-align:left">textarea</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">1000</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x8868;&#x793A;</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
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
          &#x9867;&#x5BA2;API&#x3092;&#x5B9F;&#x884C;</p>
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
      <td style="text-align:left">customerId&#x304B;&#x3089;[customerId - name]&#x3092;&#x8868;&#x793A;</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x554F;&#x5408;&#x96FB;&#x8A71;&#x756A;&#x53F7;</td>
      <td style="text-align:left">&#x6570;&#x5024;&#x306E;&#x307F;&#x4FDD;&#x5B58;&#x53EF;</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3057;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;S106_3
          &#x554F;&#x5408;&#x5C65;&#x6B74;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

**inquirySave**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 3 | 問合担当者 | staff |
| 4 | 問合電話番号 | tel |
| 5 | 問合メールアドレス | email |
| 6 | 問合題名 | title |
| 7 | 問合内容 | contents |
{% endtab %}

{% tab title="顧客API" %}
#### 使用API

customerSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |

#### セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 3 | 問合担当者 | staffName |
| 4 | 問合電話番号 | tel |
| 5 | 問合メールアドレス | email |
{% endtab %}
{% endtabs %}



