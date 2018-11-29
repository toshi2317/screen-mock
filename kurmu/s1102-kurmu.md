# S110\_2 クレーム登録

### **クレーム情報部**

{% tabs %}
{% tab title="項目制御" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">No</th>
      <th style="text-align:left">名称</th>
      <th style="text-align:left">
        <p></p>
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
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">受注先</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">list</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">題名</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">text</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">200</td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">内容</td>
      <td style="text-align:left">更新</td>
      <td style="text-align:left">textarea</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">1000</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">保存</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">表示</td>
      <td style="text-align:left">button</td>
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
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">
        <p>GETパラメータにcustomerIdが存在する場合、顧客APIを実行</p>
        <p>customerIdから[customerId - name]を表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">顧客名</td>
      <td style="text-align:left">
        <p>GETパラメータにcustomerIdが存在しない場合</p>
        <p>顧客検索ボタンを表示し、押下でS103_1 顧客一覧をPOPUP表示</p>
        <p>当画面に戻ってきた際、顧客APIを実行</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">受注先</td>
      <td style="text-align:left">受注先APIの結果[orderId - name]をリスト表示</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
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
      <td style="text-align:left">6</td>
      <td style="text-align:left">戻る</td>
      <td style="text-align:left">前の画面に戻る</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="保存API" %}
#### 使用API <a id="shi-yong-api"></a>

**claimSave**

| No |  | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
| 2 | 受注先 | orderId |
| 3 | 題名 | title |
| 4 | 内容 | contents  |
{% endtab %}

{% tab title="顧客API" %}
#### 使用API <a id="shi-yong-api-1"></a>

**customerSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |

**セット内容**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
| 1 | 顧客名 | customerName |
{% endtab %}

{% tab title="受注先API" %}
**使用API**

**orderSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | 顧客名 | customerId |
{% endtab %}
{% endtabs %}

