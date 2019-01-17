# S110\_3 クレーム編集

### クレーム情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | ID | 表示 | text | Y |  |
| 2 | 顧客名 | 表示 | text | Y |  |
| 3 | 受注ID | 表示 | text |  |  |
| 4 | 題名 | 更新 | text |  | 200 |
| 5 | 内容 | 更新 | textarea |  | 1000 |
| 6 | 保存 | 表示 | button |  |  |
| 7 | 戻る | 表示 | button |  |  |
{% endtab %}

{% tab title="起動時API" %}
**使用API**

**claimSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | claimId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | claimId |
| 2 | 顧客名 | customerName |
| 3 | 受注ID | orderId |
| 4 | 題名 | title |
| 5 | 内容 | contents |
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
      <td style="text-align:left">3</td>
      <td style="text-align:left">受注ID</td>
      <td style="text-align:left">
        <p>返却値にorderIdが存在する場合は表示</p>
        <p>存在しない場合は当項目非表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、保存されましたメッセージ表示</p>
        <p>・保存されましたメッセージ表示後、S110_3 クレーム編集画面へ遷移する</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**claimSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | claimId |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
| 3 | 受注ID | orderId |
| 4 | 題名 | title |
| 5 | 内容 | contents |
{% endtab %}
{% endtabs %}

