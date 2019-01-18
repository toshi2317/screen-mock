# S103\_1 顧客一覧

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
| 1 | 新規登録 | 押下でS103\_2 顧客登録画面へ遷移 |
| 1 | 新規登録 | 別画面からPOPUPで起動した場合、当ボタンは非表示 |
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
      <td style="text-align:left">顧客ID</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">顧客名/ふりがな</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">電話番号</td>
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
      <td style="text-align:left">検索</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">非同期CSV</td>
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
      <td style="text-align:left">6</td>
      <td style="text-align:left">検索</td>
      <td style="text-align:left">
        <p>検索APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値を一覧表示部に表示する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">CSV</td>
      <td style="text-align:left">検索結果をCSVとして出力する</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">非同期CSV</td>
      <td style="text-align:left">
        <p>押下でファイル出力保存APIを実行</p>
        <p>・検索結果をCSVとして出力する</p>
        <p>・失敗した場合、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、検索APIの返却値をに表示する</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
#### 使用API

**customerSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客id | customerId |
| 3 | 顧客名/ふりがな | name |
| 4 | 電話番号 | tel |
| 5 | メールアドレス | email |
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
      <td style="text-align:left">10</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">担当者</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
      <td style="text-align:left">メールアドレス</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
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
      <td style="text-align:left">10</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">押下でS103_3 顧客編集画面を別タブ起動する</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">POPUP表示の場合、押下で親画面に値を引き継ぐ</td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">
        <p>0 -> OFF</p>
        <p>1 -> ON</p>
        <p>と表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示パラメータ名" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 10 | ID | customerName |
| 11 | 顧客名 | name |
| 12 | ふりがな | kana |
| 13 | 電話番号 | tel |
| 14 | 担当者 | staffName |
| 15 | メールアドレス | email |
| 16 | 郵便番号 | zip |
| 17 | 都道府県 | address1 |
| 18 | 住所 | address2 |
| 19 | 無効フラグ | disableFlag |
{% endtab %}
{% endtabs %}



