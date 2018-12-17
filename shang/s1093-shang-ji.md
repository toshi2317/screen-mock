# S109\_3 売上編集

### **売上情報部**

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
| 8 | 都道府県 | 表示 | text |  |  |
| 9 | 住所 | 更新 | text |  | 300 |
| 10 | 納品先 | 更新 | list |  |  |
| 11 | 請求先 | 更新 | list |  |  |
| 12 | 請求日 | 更新 | date |  |  |
| 13 | 支払期限日 | 更新 | date |  |  |
| 14 | 区分 | 更新 | list |  |  |
{% endtab %}

{% tab title="起動時API" %}
#### 使用API① <a id="shi-yong-api"></a>

**salesDetailSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |

**セット内容（売上明細は売上明細部に記載）**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billingId |
| 12 | 請求日 | billingDate |
| 13 | 支払期限日 | paymentDate |
| 14 | 区分 | type |
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
      <td style="text-align:left">customerIdから[customerId - name]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">
        <p>入力した郵便番号から自動提案</p>
        <p>変更不可</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">9</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">
        <p>入力した郵便番号から自動提案</p>
        <p>変更可</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">納品先</td>
      <td style="text-align:left">
        <p>画面起動時に納品先APIを実行</p>
        <p>返却値に現在のlocationIdが存在する場合はデフォルトセット</p>
        <p>存在しない場合はデフォルト無し</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">請求先</td>
      <td style="text-align:left">
        <p>画面起動時に請求先APIを実行</p>
        <p>返却値に現在のlocationIdが存在する場合はデフォルトセット</p>
        <p>存在しない場合はデフォルト無し</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
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

{% tab title="納品先API" %}
#### 使用API <a id="shi-yong-api-1"></a>

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
        <p>検索結果が0件の場合、バリデーションNG</p>
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
| 15 | 明細追加 | 表示 | button |
| 16 | 明細削除 | 表示 | button |
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

### 売上明細部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 17 | チェック | 更新 | check |
| 18 | No | 表示 | text |
| 19 | 題名 | 更新 | text |
| 20 | 詳細 | 更新 | text |
| 21 | 単価 | 更新 | text |
| 22 | 数量 | 更新 | text |
| 23 | 金額 | 表示 | text |
{% endtab %}

{% tab title="起動時API" %}
**使用APIは売上情報部に記載済み**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | title |
| 20 | 詳細 | detail |
| 21 | 単価 | unitPrice |
| 22 | 数量 | count |
| 23 | 金額 | amount |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 18 | No | 画面上の連番 |
| 23 | 金額 | 単価 \* 数量 |
{% endtab %}
{% endtabs %}

### 売上明細フッダー部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 24 | 税抜金額 | 表示 | text |
| 25 | 消費税率 | 表示 | hidden |
| 26 | 消費税額 | 表示 | text |
| 27 | 税込金額 | 表示 | text |
{% endtab %}

{% tab title="起動時API" %}
**使用APIは売上情報部に記載済み**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 24 | 税抜金額 | amount |
| 25 | 消費税率 | taxRate |
| 26 | 消費税額 | tax |
| 27 | 税込金額 | totalAmount |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 24 | 税抜金額 | 売上明細部、金額の合計値 |
| 25 | 消費税率 | 画面上非表示、登録時の値を使用、変更不可で変わることはなし |
| 26 | 消費税額 | 税抜金額 \* 消費税率 |
| 27 | 税込金額 | 税抜金額 + 消費税額 |
{% endtab %}
{% endtabs %}

### ボタン部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 24 | 保存 | 表示 | button |
| 25 | 戻る | 表示 | button |
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
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、S109_3 売上編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API <a id="shi-yong-api-3"></a>

**salesSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | salesId |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
| 3 | ふりがな | customerKana |
| 4 | 電話番号 | customerTel |
| 5 | 担当者 | customerStaffName |
| 6 | メールアドレス | customerEmail |
| 7 | 郵便番号 | customerZip |
| 8 | 都道府県 | customerAddress1 |
| 9 | 住所 | customerAddress2 |
| 10 | 納品先 | locationId |
| 11 | 請求先 | billinbId |
| 12 | 請求日 | billingDate |
| 13 | 支払期限日 | paymentDate |
| 24 | 税抜合計 | amount |
| 25 | 消費税率 | taxRate |
| 26 | 消費税額 | tax |
| 27 | 税込金額 | totalAmount |
| 14 | 区分 | types |
| - | 売上明細数 | detailCount |

**売上明細（売上 1 に対して 売上明細 N）**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 題名 | title |
| 20 | 詳細 | detail |
| 21 | 単価 | unitPrice |
| 22 | 数量 | count |
| 23 | 金額 | amount |
{% endtab %}
{% endtabs %}

