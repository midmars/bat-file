# -bat 指令
COPY	/Y   不顯示確認覆寫現有檔案的提示。
		copy source[A] destination[B]



REM 用來在批次檔執行中顯示某些訊息

echo 代換參數
	 echo %1%2
 
start 啟動獨立視窗來執行指定程式

ping	-n count 要傳送的echo要求數目
		-w timeout 每個回覆逾時的時間(毫秒)
ex:
		ping -n 1 1.1.1.1 -w 120000 > nul
		ping 1.1.1.1 測試發送一個資料包 等待 如果過了12000毫秒就逾時
		
taskkill 強制結束	/F 指定要強制中止的處理程序。
					/IM   image name       指定要中止的處理程序的影像名稱。萬用字元 '*'可以用來指定所有影像名稱。
					
if(%3) neq() pause	if "變數"不等於0 pause
					neq-不等於
					EQU-等於
					LSS-小於
					LEQ-小於或等於
					GTR-大於
					GEQ-大於或等於
					
Xcopy
	複製檔案和樹狀目錄
	XCOPY source [destination] [/E][/C][/Y][/F][/EXCLUDE:file1[+file2][+file3]...]
	/E-複製目錄和子目錄，包括空目錄。
	/C-即使發生錯誤仍繼續複製。
	/Y-不提示確認是否要覆寫現有的目的地檔案。
	/F-複製時顯示完整的來源和目的地檔名。
	/EXCLUDE:file1[+file2][+file3]...
指定包含字串的檔案清單。當字串中有與欲複製的檔案之絕對路徑
任何部分相符時，
該檔案就不會複製。如果是
例如若指定一個字串 \obj\ 或 .obj，
它會分別排除 obj 目錄下的所有檔案，
以及所有具有 .obj 副檔名的檔案。


devenv VISUAL STUDIO 裡面的
		/Rebuild	根據指定的方案之組態，清除然後建置指定的方案或專案。
					

diff --summerize 只顯示會變化的檔案名
