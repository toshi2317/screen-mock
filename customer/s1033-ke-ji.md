# S103\_3 顧客編集



### 顧客情報部

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
      <td style="text-align:left"></td>
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
      <td style="text-align:left">Y</td>
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
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">50</td>
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
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">check</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">buton</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**customerSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |

#### セット内容

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
| 2 | 顧客名 | name |
| 3 | ふりがな | kana |
| 4 | 電話番号 | tel |
| 5 | 担当者 | staffName |
| 6 | メールアドレス | email |
| 7 | 郵便番号 | zip |
| 8 | 都道府県 | address1 |
| 9 | 住所 | address2 |
| 10 | 無効フラグ | disableFlag |
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
      <td style="text-align:left">11</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、保存APIの返却値をセットしたS103_3 顧客編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API

**customerSave**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
| 2 | 顧客名 | name |
| 3 | ふりがな | kana |
| 4 | 電話番号 | tel |
| 5 | 担当者 | staffName |
| 6 | メールアドレス | email |
| 7 | 郵便番号 | zip |
| 8 | 都道府県 | address1 |
| 9 | 住所 | address2 |
| 10 | 無効フラグ | disableFlag |
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

### 納品先情報ボタン部

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
      <td style="text-align:left">13</td>
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
| 13 | 新規登録 | 押下でS104\_1 納品先登録画面へ遷移 |
| 13 | 新規登録 | 遷移時、customerIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### 納品先情報一覧部

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
      <td style="text-align:left">14</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
      <td style="text-align:left">納品先名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">納品先担当者</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">20</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">21</td>
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**locationSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
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
      <td style="text-align:left">ID</td>
      <td style="text-align:left">押下でS104_2 納品先編集画面を別タブ起動</td>
    </tr>
    <tr>
      <td style="text-align:left">21</td>
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
| 14 | ID | locationId |
| 15 | 納品先名 | name |
| 16 | ふりがな | kana |
| 17 | 納品先担当者 | staffName |
| 18 | 郵便番号 | zip |
| 19 | 都道府県 | address1 |
| 20 | 住所 | address2 |
| 21 | 無効フラグ | disableFlag |
{% endtab %}
{% endtabs %}

### 請求先情報ボタン部

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
      <td style="text-align:left">22</td>
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
| 22 | 新規登録 | 押下でS105\_1 請求先登録画面へ遷移 |
| 22 | 新規登録 | 遷移時、customerIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### 請求先情報一覧部

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
      <td style="text-align:left">23</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">24</td>
      <td style="text-align:left">請求先名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">25</td>
      <td style="text-align:left">ふりがな</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">26</td>
      <td style="text-align:left">請求先担当者</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">27</td>
      <td style="text-align:left">郵便番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">28</td>
      <td style="text-align:left">都道府県</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">29</td>
      <td style="text-align:left">住所</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">30</td>
      <td style="text-align:left">無効フラグ</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**billingSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
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
      <td style="text-align:left">ID</td>
      <td style="text-align:left">押下でS105_2 請求先編集画面を別タブ起動</td>
    </tr>
    <tr>
      <td style="text-align:left">30</td>
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
| 23 | ID | billingId |
| 24 | 請求先名 | name |
| 25 | ふりがな | kana |
| 26 | 請求先担当者 | staffName |
| 27 | 郵便番号 | zip |
| 28 | 都道府県 | address1 |
| 29 | 住所 | address2 |
| 30 | 無効フラグ | disableFlag |
{% endtab %}
{% endtabs %}

### 問合履歴情報ボタン部

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
      <td style="text-align:left">31</td>
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
| 31 | 新規登録 | 押下でS106\_2 問合履歴登録画面へ遷移 |
| 31 | 新規登録 | 遷移時、customerIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### 問合履歴情報一覧部

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
      <td style="text-align:left">32</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">33</td>
      <td style="text-align:left">担当者</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">34</td>
      <td style="text-align:left">電話番号</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">35</td>
      <td style="text-align:left">メールアドレス</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">36</td>
      <td style="text-align:left">題名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">37</td>
      <td style="text-align:left">内容</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**inquirySearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 32 | ID | 押下でS106\_3 問合履歴編集画面を別タブ起動 |
{% endtab %}

{% tab title="表示パラメータ名" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 32 | ID | inquiryId |
| 33 | 担当者 | staff |
| 34 | 電話番号 | tel |
| 35 | メールアドレス | email |
| 36 | 題名 | title |
| 37 | 内容 | contents |
{% endtab %}
{% endtabs %}

### 見積情報ボタン部

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
      <td style="text-align:left">38</td>
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
| 38 | 新規登録 | 押下でS107\_2 見積登録画面へ遷移 |
| 38 | 新規登録 | 遷移時、customerIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### 見積情報一覧部

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
      <td style="text-align:left">39</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">40</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">41</td>
      <td style="text-align:left">有効期限</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">42</td>
      <td style="text-align:left">税抜合計</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">43</td>
      <td style="text-align:left">納品予定日</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**quotationSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 39 | ID | 押下でS107\_3 見積編集画面を別タブ起動 |
{% endtab %}

{% tab title="表示パラメータ名" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 39 | ID | quotationId |
| 40 | 見積日 | quotationDate |
| 41 | 有効期限 | quotationExpirationDate |
| 42 | 税抜合計 | amount |
| 44 | 納品予定日 | daliveryDate |
{% endtab %}
{% endtabs %}

### 受注情報ボタン部

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
      <td style="text-align:left">45</td>
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
| 44 | 新規登録 | 押下でS108\_2 受注登録画面へ遷移 |
| 44 | 新規登録 | 遷移時、customerIdをGETパラメータにセットする |
{% endtab %}
{% endtabs %}

### 受注情報一覧部

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
      <td style="text-align:left">45</td>
      <td style="text-align:left">ID</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">textlink</td>
    </tr>
    <tr>
      <td style="text-align:left">46</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">47</td>
      <td style="text-align:left">納品日</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">48</td>
      <td style="text-align:left">契約金額</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
    <tr>
      <td style="text-align:left">49</td>
      <td style="text-align:left">区分</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
#### 使用API

**orderSearch**

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | customerId |
{% endtab %}

{% tab title="詳細仕様" %}
| No | 名称 | 表示条件/仕様 |
| :--- | :--- | :--- |
| 45 | ID | 押下でS108\_3 受注編集画面を別タブ起動 |
{% endtab %}

{% tab title="表示パラメータ名" %}
| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 45 | ID | orderId |
| 46 | 受注日 | orderDate |
| 47 | 納品日 | deliveryDate |
| 48 | 契約金額 | contractAmount |
| 49 | 区分 | types |
{% endtab %}
{% endtabs %}

