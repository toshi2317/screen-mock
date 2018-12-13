# S107\_2 見積登録

### 見積情報部

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
      <td style="text-align:left">顧客検索</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">担当者</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">メールアドレス</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">100</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">8</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">list</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">300</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">納品先</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">list</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">請求先</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">list</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">見積有効期限</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">納品予定日</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">date</td>
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">顧客検索</td>
      <td style="text-align:left">
        <p>GETパラメータにcustomerIdが存在する場合、
          <br />顧客API、納品先API、請求先APIを実行</p>
        <p>当ボタン非表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">顧客検索</td>
      <td style="text-align:left">
        <p>押下でS103_1 顧客一覧をPOPUP表示</p>
        <p>当画面に戻ってきた際、</p>
        <p>顧客API、納品先API、請求先APIを実行</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">選択されている顧客の[customerId - name]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">ひらがなのみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">数値のみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">数値のみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">xxx-xxxx という形のみ許容</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">納品先</td>
      <td style="text-align:left">納品先APIの結果[locationId - name]をリスト表示</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">請求先</td>
      <td style="text-align:left">請求先APIの結果[billingId - name]をリスト表示</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">当日を自動提案</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">見積有効期限</td>
      <td style="text-align:left">当日 + 1ヶ月の月末日を自動提案</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="顧客API" %}
#### 使用API

**customerSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |

#### 　セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | name |
| 3 | ふりがな | kana |
| 4 | 電話番号 | tel |
| 5 | 担当者 | staffName |
| 6 | メールアドレス | email |
| 7 | 郵便番号 | zip |
| 8 | 都道府県 | address1 |
| 9 | 住所 | address2 |
{% endtab %}

{% tab title="納品先API" %}
#### 使用API

**locationSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
{% endtab %}

{% tab title="請求先API" %}
#### 使用API

**billingSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
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
      <td style="text-align:left">7</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">更新時</td>
      <td style="text-align:left">addressSearch</td>
      <td style="text-align:left">
        <p>入力した郵便番号を[zipCode]にセットする</p>
        <p>返却された情報を元に[都道府県][住所]項目を更新する</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

### 見積明細ヘッダー部

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
      <td style="text-align:left">15</td>
      <td style="text-align:left">明細追加</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">明細削除</td>
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
      <td style="text-align:left">15</td>
      <td style="text-align:left">明細追加</td>
      <td style="text-align:left">見積明細部、一番下に1行明細を追加する</td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">明細削除</td>
      <td style="text-align:left">
        <p>確認ダイアログを表示し、見積明細部、チェック = ON</p>
        <p>の行を削除する</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

### 見積明細部

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
      <th style="text-align:left">文字数</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">チェック</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">check</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">No</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">題名</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">20</td>
      <td style="text-align:left">詳細</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">300</td>
    </tr>
    <tr>
      <td style="text-align:left">21</td>
      <td style="text-align:left">単価</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">22</td>
      <td style="text-align:left">数量</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">23</td>
      <td style="text-align:left">金額</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 18 | No | 画面上の連番 |
| 23 | 金額 | 単価 \* 数量 |
{% endtab %}
{% endtabs %}

### 見積明細フッダー部

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
      <td style="text-align:left">24</td>
      <td style="text-align:left">税抜金額</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">消費税率</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">hidden</td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
      <td style="text-align:left">消費税額</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">税込金額</td>
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
      <td style="text-align:left">24</td>
      <td style="text-align:left">税抜金額</td>
      <td style="text-align:left">見積明細部、金額の合計値</td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">消費税率</td>
      <td style="text-align:left">
        <p>画面上非表示、消費税率の取得方法は消費税率検索API参照</p>
        <p>見積日を元にtax_rateを取得する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
      <td style="text-align:left">消費税額</td>
      <td style="text-align:left">税抜金額 * 消費税率</td>
    </tr>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">税込金額</td>
      <td style="text-align:left">税抜金額 + 消費税額</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

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
      <td style="text-align:left">28</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
    </tr>
    <tr>
      <td style="text-align:left">29</td>
      <td style="text-align:left">戻る</td>
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
      <td style="text-align:left">28</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、登録完了しましたメッセージ表示</p>
        <p>・登録完了しましたメッセージ表示後、S107_3 見積編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">29</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

**quotationSave**

#### 見積

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billinbId |
| 12 | 見積日 | quotationDate |
| 13 | 見積有効期限 | quotationExpirationDate |
| 14 | 納品予定日 | deliveryDate |
| 24 | 税抜合計 | amount |
| 25 | 消費税率 | taxRate |
| 26 | 消費税額 | tax |
| 27 | 税込金額 | totalAmount |
| - | 見積明細数 | detailCount |

#### 見積明細（見積 1 に対して 見積明細 N）

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | detailTitle |
| 20 | 詳細 | detailDetail |
| 21 | 単価 | detailUnitPrice |
| 22 | 数量 | detailCount |
| 23 | 金額 | detailAmount |
{% endtab %}
{% endtabs %}



