# J102 受注集計

orderDateFrom = 実行現在日付 - Job env設定に基づく日付

orderDateTo = 実行現在日付

をセットしたorderSearchを実行

返却されたデータより、orderDate、type単位で件数と金額を集計する

集計結果をorderSummarySave APIにセットし、保存を行う

（orderDate、type単位でAPIを実行）

