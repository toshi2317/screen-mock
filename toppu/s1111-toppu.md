# S111\_1 トップ

#### 見積件数グラフ部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 1 | 見積件数 | 表示 | graph |
| 2 | 見積日 | 表示 | graph |
| 3 | 見積件数集計データ\(今週\) | 表示 | graph |
| 4 | 見積件数集計データ\(先週\) | 表示 | graph |
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
      <td style="text-align:left">見積件数</td>
      <td style="text-align:left">
        <p>見積件数縦軸とする。</p>
        <p>単位は件、100件ごとに目盛表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">2</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">
        <p>見積日横軸とする。</p>
        <p>単位は月日、当日 - 6日~当日の7日を1日毎表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">見積件数集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日 - 6日~当日の1日毎の見積件数集計したもの緑でBar Chart表示</p>
        <p>マウスバーで件数表示</p>
        <p>見積件数取得方法はJ101 見積集計参照、API叩いて出たsummaryCountの値をBar Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">見積件数集計データ(先週)</td>
      <td style="text-align:left">
        <p>今週の日付-7日の1日毎の見積件数集計したもの青でBar Chart表示</p>
        <p>マウスバーで件数表示</p>
        <p>見積件数取得方法はJ101 見積集計参照、API叩いて出たsummaryCountの値をBar Chart表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
**使用API**

quotationsummary

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 見積日 | quotationDate |
| 3 | 見積件数集計データ\(今週\) | summaryCount |
| 4 | 見積件数集計データ\(先週\) | summaryCount |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

quotationsummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 2 | 見積日 | quotationDate |
| 3 | 見積件数集計データ\(今週\) | summaryCount |
| 4 | 見積件数集計データ\(先週\) | summaryCount |
{% endtab %}
{% endtabs %}

#### 見積金額グラフ部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 5 | 見積金額 | 表示 | graph |
| 6 | 見積日 | 表示 | graph |
| 7 | 見積金額集計データ\(今週\) | 表示 | graph |
| 8 | 見積金額集計データ\(先週\) | 表示 | graph |
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
      <td style="text-align:left">5</td>
      <td style="text-align:left">見積金額</td>
      <td style="text-align:left">
        <p>見積金額縦軸とする。</p>
        <p>単位は円、100万円ごとに目盛表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">
        <p>見積日横軸とする。</p>
        <p>単位は月日、当日 - 6日~当日の7日を1日毎表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">見積金額集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日 - 6日~当日の1日毎の見積金額緑線でLine Chart表示</p>
        <p>マウスバーで金額表示</p>
        <p>見積件数取得方法はJ101 見積集計参照、API叩いて出たsummaryAmountの値をBar Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">見積金額集計データ(先週)</td>
      <td style="text-align:left">
        <p>今週の日付-7日の1日毎の見積金額青線でLine Chart表示</p>
        <p>マウスバーで金額表示</p>
        <p>見積件数取得方法はJ101 見積集計参照、API叩いて出たsummaryAmountの値をBar Chart表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
**使用API**

quotationSummary

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 6 | 見積日 | quotationDate |
| 7 | 見積金額集計データ\(今週\) | summaryAmount |
| 8 | 見積金額集計データ\(先週\) | summaryAmount |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

quotationSummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 6 | 見積日 | quotationDate |
| 7 | 見積金額集計データ\(今週\) | summaryAmount |
| 8 | 見積金額集計データ\(先週\) | summaryAmount |
{% endtab %}
{% endtabs %}

#### 受注件数グラフ部

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 9 | 受注件数 | 表示 | graph |
| 10 | 受注日 | 表示 | graph |
| 11 | 受注件数集計データ\(今週\) | 表示 | graph |
| 12 | 受注件数集計データ\(先週\) | 表示 | graph |
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
      <td style="text-align:left">9</td>
      <td style="text-align:left">受注件数</td>
      <td style="text-align:left">
        <p>受注件数縦軸とする。</p>
        <p>単位は件、100件ごとに目盛表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">10</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">
        <p>受注日横軸とする。</p>
        <p>単位は月日、当日 - 6日~当日の7日を1日毎表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">受注件数集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日 - 6日~当日の1日毎の受注件数集計したもの緑線でLine Chart2表示</p>
        <p>マウスバーで件数表示</p>
        <p>受注件数取得方法はJ102 受注集計参照、API叩いて出たsummaryCountの値をBar Chart2表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">受注件数集計データ(先週)</td>
      <td style="text-align:left">
        <p>今週の日付-7日の1日毎の受注件数集計したもの青線でLine Chart2表示</p>
        <p>マウスバーで件数表示</p>
        <p>受注件数取得方法はJ102 受注集計参照、API叩いて出たsummaryCountの値をBar Chart2表示</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
**使用API**

orderSummary

| **No** | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 10 | 受注日 | orderDate |
| 11 | 受注件数集計データ\(今週\) | summaryCount |
| 12 | 受注件数集計データ\(先週\) | summaryCount |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

ordersummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 10 | 受注日 | orderDate |
| 11 | 受注件数集計データ\(今週\) | summaryCount |
| 12 | 受注件数集計データ\(先週\) | summaryCount |
{% endtab %}
{% endtabs %}

#### 受注金額グラフ部\(前月\)

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 13 | 受注日 | 表示 | text |
| 14 | 受託 | 表示 | graph |
| 15 | SES | 表示 | graph |
| 16 | その他 | 表示 | graph |
| 17 | 受注金額 | 表示 | graph |
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
      <td style="text-align:left">13</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">当月の前の月表示</td>
    </tr>
    <tr>
      <td style="text-align:left">14</td>
      <td style="text-align:left">受託</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>実行現在月の前月、type=1指定してAPI叩いて出た summaryCountractAmountの値を緑でDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
      <td style="text-align:left">SES</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>実行現在月の前月、type=2指定してAPI叩いて出た summaryCountractAmountの値を青でDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">その他</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>実行現在月の前月、type=NULL指定してAPI叩いて出た summaryCountractAmountの値をグレーでDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">17</td>
      <td style="text-align:left">受注金額</td>
      <td style="text-align:left">マウスバーで色ごとの受注金額集計額、区分名表示</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
**使用API**

ordersummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 13 | 受注日 | orderDate |
| 14 | 受託 | types |
| 14 | 受託 | sammaryContractAmount |
| 15 | SES | types |
| 15 | SES | sammaryContractAmount |
| 16 | その他 | types |
| 16 | その他 | sammaryContractAmount |
| 17 | 受注金額 | sammaryContractAmount |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

ordersummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 14 | 受託 | types |
| 14 | 受託 | sammaryContractAmount |
| 15 | SES | types |
| 15 | SES | sammaryContractAmount |
| 16 | その他 | types |
| 16 | その他 | sammaryContractAmount |
| 17 | 受注金額 | sammaryContractAmount |
{% endtab %}
{% endtabs %}

#### 受注金額グラフ部\(当月\)

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 18 | 受注日 | 表示 | text |
| 19 | 受託 | 表示 | graph |
| 20 | SES | 表示 | graph |
| 21 | その他 | 表示 | graph |
| 22 | 受注金額 | 表示 | graph |
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
      <td style="text-align:left">18</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">当月の月表示</td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">受託</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>当月現在月、type=1指定してAPI叩いて出た summaryCountractAmountの値を緑でDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">20</td>
      <td style="text-align:left">SES</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>実行現在月、type=2指定してAPI叩いて出た summaryCountractAmountの値を青でDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">21</td>
      <td style="text-align:left">その他</td>
      <td style="text-align:left">
        <p>受注金額集計額取得方法はJ102 受注集計参照</p>
        <p>実行現在月、type=NULL指定してAPI叩いて出た summaryCountractAmountの値をグレーでDonut Chart表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">22</td>
      <td style="text-align:left">受注金額</td>
      <td style="text-align:left">マウスバーで色ごとの受注金額集計額、区分名表示</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="起動時API" %}
**使用API**

ordersummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 18 | 受注日 | orderDate |
| 19 | 受託 | types |
| 19 | 受託 | sammaryContractAmount |
| 20 | SES | types |
| 20 | SES | sammaryContractAmount |
| 21 | その他 | types |
| 21 | その他 | sammaryContractAmount |
| 22 | 受注金額 | sammaryContractAmount |
{% endtab %}

{% tab title="表示API" %}
#### 使用API

ordersummary

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 19 | 受託 | types |
| 19 | 受託 | sammaryContractAmount |
| 20 | SES | types |
| 20 | SES | sammaryContractAmount |
| 21 | その他 | types |
| 21 | その他 | sammaryContractAmount |
| 22 | 受注金額 | sammaryContractAmount |
{% endtab %}
{% endtabs %}

