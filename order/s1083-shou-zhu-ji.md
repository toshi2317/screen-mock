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
| 10 | 納品先 | 更新 | list |  |  |
| 11 | 請求先 | 更新 | list |  |  |
| 12 | 見積ID | 更新 | text |  |  |
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
      <th style="text-align:left">名称</th>
      <th style="text-align:left">表示条件/仕様</th>
    </tr>
  </thead>
  <tbody>
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
      <td style="text-align:left">12</td>
      <td style="text-align:left">見積ID</td>
      <td style="text-align:left">
        <p>見積ID = NULLの場合は当項目非表示</p>
        <p>変更不可</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">区分</td>
      <td style="text-align:left">
        <p>-</p>
        <p>1.受託</p>
        <p>2.SES リスト値表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、S108_3 受注編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
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

