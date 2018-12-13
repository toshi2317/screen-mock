# S104\_2 納品先編集

### 納品先情報部

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
      <th style="text-align:left">必須</th>
      <th style="text-align:left">文字数</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">納品先名</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">納品先担当者</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">8</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">300</td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">check</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**locationSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | locationId |

#### セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | locationId |
| 2 | 顧客名 | customerName |
| 3 | 納品先名 | name |
| 4 | ふりがな | kana |
| 5 | 納品先担当者 | staffName |
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">customerIdから[customerId - customerName]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">ひらがなのみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">数値のみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">xxx-xxxx という形のみ許容</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">
        <p>入力した郵便番号から自動提案</p>
        <p>変更不可</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">
        <p>入力した郵便番号から自動提案</p>
        <p>変更可</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、S104_2 納品先編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

locationSave

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | locationId |
| 2 | 顧客名 | customerId |
| 3 | 納品先名 | name |
| 4 | ふりがな | kana |
| 5 | 納品先担当者 | staffName |
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">タイミング</th>
      <th style="text-align:left">API</th>
      <th style="text-align:left">内容</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">更新時</td>
      <td style="text-align:left">addressSearch</td>
      <td style="text-align:left">
        <p>入力した郵便番号を[zipCode]にセットする</p>
        <p>返却された情報を元に[都道府県][住所]項目を更新する</p>
        <p>検索結果が0件の場合、バリデーションNG</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

