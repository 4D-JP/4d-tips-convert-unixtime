# 4d-tips-convert-unixtime
現在のUNIX時間を返すメソッドとUNIX時間を日付と時間に変換するメソッド

```4d
/* 
	
	現在のUNIX時間を返す
	
*/

C_OBJECT($time)

$time:=CURRENT_UNIXTIME 

ALERT(New collection($time.timestamp;$time.ms).join("."))

/* 
	
	UNIX時間をローカル日付/時間およびUTC日付時間に変換する
	
*/

$time:=CONVERT_UNIXTIME ($time.timestamp)
```
