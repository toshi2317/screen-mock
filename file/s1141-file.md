# S114\_1 ファイル出力状況一覧

### 検索条件部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | ID | 更新 | text |
| 2 | ステータス | 更新 | list |
| 3 | 出力依頼日\(From\) | 更新 | date |
| 4 | 出力依頼日\(To\) | 更新 | date |
| 5 | クリア | 表示 | button |
| 6 | 検索 | 表示 | button |
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
      <td style="text-align:left">ステータス</td>
      <td style="text-align:left">
        <p>--</p>
        <p>1.待機中</p>
        <p>2.実行中</p>
        <p>3.完了</p>
        <p>9.失敗</p>
        <p>リスト値表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">出力依頼日(From)</td>
      <td style="text-align:left">当日を自動提案</td>
    </tr>
    <tr>
      <td style="text-align:left">5</td>
      <td style="text-align:left">クリア</td>
      <td style="text-align:left">検索条件部をデフォルトの状態に戻す</td>
    </tr>
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
  </tbody>
</table>
{% endtab %}

{% tab title="検索API" %}
**使用API**

**fileStatusSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 1 | ID | fileStatusId |
| 2 | ステータス | status |
| 3 | 出力依頼日\(From\) | createdAtFrom |
| 4 | 出力依頼日\(To\) | createdAtTo |
{% endtab %}
{% endtabs %}

### 一覧情報部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 5 | ID | 表示 | text |
| 6 | SQSキューID | 表示 | text |
| 7 | ファイル | 表示 | textlink |
| 8 | ステータス | 表示 | text |
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
      <td style="text-align:left">7</td>
      <td style="text-align:left">ファイル</td>
      <td style="text-align:left">押下でCSVファイル出力</td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">ステータス</td>
      <td style="text-align:left">
        <p>1.待機中 2.実行中 3.完了 9.失敗</p>
        <p>ステータスの値の文言表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
**使用API**

**fileStatusSearch**

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 5 | ID | fileStatusId |
| 6 | SQSキューID | sqsId |
| 7 | ファイル | filePath |
| 8 | ステータス | status |
{% endtab %}
{% endtabs %}

