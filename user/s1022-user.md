# S102\_2 ユーザー登録

### ユーザー情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | メールアドレス | 更新 | text |  |  |
| 2 | 権限 | 更新 | list |  |  |
| 3 | パスワード | 更新 | password |  |  |
| 4 | パスワード変更ボタン | 表示 | check |  |  |
| 5 | 保存 | 表示 | button |  |  |
| 6 | 戻る | 表示 | button |  |  |
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
      <td style="text-align:left">&#x6A29;&#x9650;</td>
      <td style="text-align:left">
        <p>1:&#x30B7;&#x30B9;&#x30C6;&#x30E0;&#x7BA1;&#x7406;&#x8005;</p>
        <p>&#x30EA;&#x30B9;&#x30C8;&#x5024;&#x8868;&#x793A;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">&#x30D1;&#x30B9;&#x30EF;&#x30FC;&#x30C9;&#x5909;&#x66F4;&#x30DC;&#x30BF;&#x30F3;</td>
      <td
      style="text-align:left">&#x30C1;&#x30A7;&#x30C3;&#x30AF;&#x30DC;&#x30BF;&#x30F3;&#x62BC;&#x4E0B;&#x3067;&#x5909;&#x66F4;&#x4E0D;&#x53EF;or&#x53EF;</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">&#x4FDD;&#x5B58;</td>
      <td style="text-align:left">
        <p>&#x4FDD;&#x5B58;API&#x3092;&#x5B9F;&#x884C;</p>
        <p>&#x30FB;&#x5931;&#x6557;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x5F53;&#x753B;&#x9762;&#x306B;&#x6B62;&#x307E;&#x308A;&#x3001;API&#x304B;&#x3089;&#x8FD4;&#x5374;&#x3055;&#x308C;&#x305F;</p>
        <p>&#x30A8;&#x30E9;&#x30FC;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x3092;&#x8868;&#x793A;&#x3059;&#x308B;</p>
        <p>&#x30FB;&#x6210;&#x529F;&#x3057;&#x305F;&#x5834;&#x5408;&#x3001;&#x767B;&#x9332;&#x5B8C;&#x4E86;&#x3055;&#x308C;&#x307E;&#x3057;&#x305F;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;</p>
        <p>&#x30FB;&#x30E1;&#x30C3;&#x30BB;&#x30FC;&#x30B8;&#x8868;&#x793A;&#x5F8C;&#x3001;&#x4FDD;&#x5B58;API&#x306E;&#x8FD4;&#x5374;&#x5024;&#x3092;&#x30BB;&#x30C3;&#x30C8;&#x3057;&#x305F;S102_3
          &#x30E6;&#x30FC;&#x30B6;&#x30FC;&#x7DE8;&#x96C6;&#x753B;&#x9762;&#x3078;&#x9077;&#x79FB;&#x3059;&#x308B;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">&#x623B;&#x308B;</td>
      <td style="text-align:left">&#x524D;&#x306E;&#x753B;&#x9762;&#x306B;&#x623B;&#x308B;</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
**保存API**

**userSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | メールアドレス | email |
| 2 | 権限 | userFlag |
| 3 | パスワード | pass |
{% endtab %}
{% endtabs %}

