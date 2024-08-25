git --version   //查看git版本

git config --global user.name "xxxxxxxxxxx" //設定作者名稱
git config --global user.email "xxxxxxx@gmail.com"  //設定信箱

git init    //初始化，建置.git

git add note.md //將note.md加入追蹤
git add note.md note1.md
git add *.*
git add .

git status  //查看狀態

git commit -m "第一次commit"    //建立備份

git log //檢視過往快照，按下"q"退出
git log --oneline

git diff    //在執行 git commit 之前，確認進行了那些變更
git diff commit   //當前分支與不同分支進行比較，git log 獲得commit
git diff commit1 commit2    //兩分支進行比較，commit1較舊
git diff af3f194 -- note.md //指定檔案看commit(af3f194)前後之差異

