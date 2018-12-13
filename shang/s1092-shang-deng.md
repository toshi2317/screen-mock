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
| 7 | 都道府県 | 更新 | text |  |  |
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">選択されている顧客の[customerId - name]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">ひらがなのみ保存可能</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">数値のみ保存可能</td>
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
      <td style="text-align:left">9</td>
      <td style="text-align:left">納品先</td>
      <td style="text-align:left">納品先APIの結果[locationId - name]をリスト表示</td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">請求先</td>
      <td style="text-align:left">請求先APIの結果[billingId - name]をリスト表示</td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">請求日</td>
      <td style="text-align:left">当日を自動提案</td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">支払期限日</td>
      <td style="text-align:left">当日 + 1ヶ月の月末日を自動提案</td>
    </tr>
    <tr>
      <td style="text-align:left">13</td>
      <td style="text-align:left">区分</td>
      <td style="text-align:left">
        <p>-</p>
        <p>1.受託</p>
        <p>2.SES リスト値表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="顧客API" %}
**使用API**

**customerSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
| 1 | 顧客名 | name |
| 2 | ふりがな | kana |
| 3 | 電話番号 | tel |
| 4 | 担当者 | staffName |
| 5 | メールアドレス | email |
| 6 | 郵便番号 | zip |
| 7 | 都道府県 | address1 |
| 8 | 住所 | address2 |
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">明細追加</td>
      <td style="text-align:left">見積明細部、一番下に1行明細を追加する</td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">23</td>
      <td style="text-align:left">税抜金額</td>
      <td style="text-align:left">売上明細部、金額の合計値</td>
    </tr>
    <tr>
      <td style="text-align:left">24</td>
      <td style="text-align:left">消費税率</td>
      <td style="text-align:left">
        <p>画面上非表示、消費税率の取得方法は消費税率検索API参照</p>
        <p>請求日を元にtax_rateを取得する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">消費税額</td>
      <td style="text-align:left">税抜金額 * 消費税率</td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、登録完了しましたメッセージ表示</p>
        <p>・登録完了しましたメッセージ表示後、S109_3 売上編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">28</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
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

