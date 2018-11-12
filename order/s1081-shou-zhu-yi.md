# S108\_1 受注一覧

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p>更新</p>
        <p>表示</p>
      </th>
      <th style="text-align:left">部品種類</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">新規登録</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 1 | 新規登録 | 押下でS107\_1 受注登録画面へ遷移 |
{% endtab %}
{% endtabs %}

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p>更新</p>
        <p>表示</p>
      </th>
      <th style="text-align:left">部品種類</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">見積ID</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">メールアドレス</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">受注日(From)</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">受注日(To)</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">納品日(From)</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">納品日(To)</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">区分</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">check</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">
        <p>検索APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値を一覧表示部に表示する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">検索結果をCSVとして出力する</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
#### 使用API

orderSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerName |
| 3 | 電話番号 | customerTel |
| 4 | 見積ID | quotationId |
| 5 | メールアドレス | customerEmail |
| 6 | 受注日\(From\) | orderDateFrom |
| 7 | 受注日\(To\) | orderDateTo |
| 8 | 納品日\(From\) | deliveryDateFrom |
| 9 | 納品日\(To\) | deliveryDateTo |
| 10 | 区分 | types |
{% endtab %}
{% endtabs %}

### 一覧表示部

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p>更新</p>
        <p>表示</p>
      </th>
      <th style="text-align:left">部品種類</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">顧客ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">見積ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">メールアドレス</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">契約金額</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">区分</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
|  |  |  |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

orderSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
|  |  |  |
{% endtab %}
{% endtabs %}

