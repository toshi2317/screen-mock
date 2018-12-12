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
        <p>単位は月日、1日ごとにその日の週の月日を表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">3</td>
      <td style="text-align:left">見積件数集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日の週の日毎の見積件数集計したもの赤でBar Chart表示</p>
        <p>マウスバーで件数表示</p>
        <p>quotationDateFrom,quotationDateTo見積日今週ででセットしてAPI叩いて出たdataCountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">4</td>
      <td style="text-align:left">見積件数集計データ(先週)</td>
      <td style="text-align:left">
        <p>先週の週の日毎の見積件数集計したものグレーでBar Chart表示</p>
        <p>マウスバーで件数表示</p>
        <p>quotationDateFrom,quotationDateTo見積日先週ででセットしてAPI叩いて出たdataCountの値</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

quotationSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 3 | 見積件数集計データ\(今週\) | dataCount |
| 4 | 見積件数集計データ\(先週\) | dataCount |
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
        <p>単位は万円、100万円ごとに目盛表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">6</td>
      <td style="text-align:left">見積日</td>
      <td style="text-align:left">
        <p>見積日横軸とする。</p>
        <p>単位は月日、1日ごとにその日の週の月日を表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">7</td>
      <td style="text-align:left">見積金額集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日の週の日毎の見積金額赤線でLine Chart表示</p>
        <p>マウスバーで金額表示</p>
        <p>quotationDateFrom,quotationDateTo見積日今週ででセットしてAPI叩いて出たsummaryAmountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">8</td>
      <td style="text-align:left">見積金額集計データ(先週)</td>
      <td style="text-align:left">
        <p>先週の週の日毎の見積金額グレー線でLine Chart表示</p>
        <p>マウスバーで金額表示</p>
        <p>quotationDateFrom,quotationDateTo見積日先週ででセットしてAPI叩いて出たsummaryAmountの値</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

quotationSearch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
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
        <p>単位は月日、1日ごとにその日の週の月日を表示</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">11</td>
      <td style="text-align:left">受注件数集計データ(今週)</td>
      <td style="text-align:left">
        <p>当日の週の日毎の受注件数集計したもの赤線でLine Chart2表示</p>
        <p>マウスバーで件数表示</p>
        <p>orderDateFrom,orderDateTo受注日今週ででセットしてAPI叩いて出たdataCountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">12</td>
      <td style="text-align:left">受注件数集計データ(先週)</td>
      <td style="text-align:left">
        <p>先週の週の日毎の受注件数集計したものグレー線でLine Chart2表示</p>
        <p>マウスバーで件数表示</p>
        <p>orderDateFrom,orderDateTo受注日でセットしてAPI叩いて出たdataCountの値</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

orderserch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 11 | 受注件数集計データ\(今週\) | dataCount |
| 12 | 受注件数集計データ\(先週\) | dataCount |
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
| 16 | 受注金額 | 表示 | graph |
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
        <p>types=1の前月の受注金額集計額を緑でDonut Chart表示</p>
        <p>type=1指定してAPI叩いて出た summaryCountractAmountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">15</td>
      <td style="text-align:left">SES</td>
      <td style="text-align:left">
        <p>types=2の前月の受注金額集計額を青でDonut Chart表示</p>
        <p>type=2指定してAPI叩いて出た summaryCountractAmountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">16</td>
      <td style="text-align:left">受注金額</td>
      <td style="text-align:left">マウスバーで色ごとの受注金額集計額、区分名表示</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

orderserch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 14 | 受託 | sammaryContractAmount |
| 15 | SES | sammaryContractAmount |
| 16 | 受注金額 | sammaryContractAmount |
{% endtab %}
{% endtabs %}

#### 受注金額グラフ部\(当月\)

{% tabs %}
{% tab title="項目制御" %}
| No | 名称 | 更新/表示 | 部品種類 |
| :--- | :--- | :--- | :--- |
| 17 | 受注日 | 表示 | text |
| 18 | 受託 | 表示 | graph |
| 19 | SES | 表示 | graph |
| 20 | 受注金額 | 表示 | graph |
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
      <td style="text-align:left">17</td>
      <td style="text-align:left">受注日</td>
      <td style="text-align:left">当月の月表示</td>
    </tr>
    <tr>
      <td style="text-align:left">18</td>
      <td style="text-align:left">受託</td>
      <td style="text-align:left">
        <p>types=1の当月の受注金額集計額を緑でDonut Chart表示</p>
        <p>type=1指定してAPI叩いて summaryCountractAmountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">19</td>
      <td style="text-align:left">SES</td>
      <td style="text-align:left">
        <p>types=2の当月の受注金額集計額を青でDonut Chart表示</p>
        <p>type=2指定してAPI叩いて summaryCountractAmountの値</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">20</td>
      <td style="text-align:left">受注金額</td>
      <td style="text-align:left">マウスバーで色ごとの受注金額集計額、区分名表示</td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="表示API" %}
#### 使用API

orderserch

| No | 名称 | パラメータ名 |
| :--- | :--- | :--- |
| 18 | 受託 | sammaryContractAmount |
| 19 | SES | sammaryContractAmount |
| 20 | 受注金額 | sammaryContractAmount |
{% endtab %}
{% endtabs %}

