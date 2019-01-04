# S110\_2 クレーム登録

### **クレーム情報部**

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 | 必須 | 文字数 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 顧客検索 | 表示 | button | Y |  |
| 2 | 顧客名 | 表示 | text | Y |  |
| 3 | 受注ID検索ボタン | 表示 | button | Y |  |
| 4 | 受注ID | 表示 | text |  |  |
| 5 | 題名 | 更新 | text |  | 200 |
| 6 | 内容 | 更新 | textarea |  | 1000 |
| 7 | 保存 | 表示 | button |  |  |
| 8 | 戻る | 表示 | button |  |  |
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
        <p>GETパラメータにcustomerIdが存在する場合、 顧客API、受注先APIを実行</p>
        <p>当ボタン非表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">顧客検索</td>
      <td style="text-align:left">
        <p>GETパラメータにcustomerIdが存在しない場合</p>
        <p>顧客検索ボタンを表示し、押下でS103_1 顧客一覧をPOPUP表示</p>
        <p>当画面に戻ってきた際、顧客APIを実行</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">選択されている顧客の[customerId - name]を表示</td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">
        <p>受注ID</p>
        <p>検索</p>
        <p>ボタン</p>
      </td>
      <td style="text-align:left">
        <p>顧客選択された時点で表示</p>
        <p>受注ID検索ボタン押下でS108_1受注一覧画面選択された顧客の受注情報POPUP表示</p>
        <p>ID押下で当画面遷移、受注ID自動提案</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">
        <p>保存APIを実行</p>
        <p>・失敗した場合、当画面に止まり、APIから返却された</p>
        <p>エラーメッセージを表示する</p>
        <p>・成功した場合、登録完了しましたメッセージ表示</p>
        <p>・登録完了しましたメッセージ表示後、S110_3 クレーム編集画面へ遷移する</p>
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
#### 使用API <a id="shi-yong-api"></a>

**claimSave**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 3 | 受注ID | orderId |
| 4 | 題名 | title |
| 5 | 内容 | contents  |
{% endtab %}

{% tab title="顧客API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**customerSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 顧客名 | customerId |
| 2 | 顧客名 | customerName |
{% endtab %}
{% endtabs %}

