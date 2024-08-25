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

git checkout commit -- temp.md  //修改temp.md，至commit快照
git reset --hard commit //注意！相較於前者，他不會留下更改紀錄，前者像是修改成過去某版
                        //後者是回到過去，所以會損失原本回到過去的版本更改紀錄


//刪除檔案依然需要git add，因為git是追蹤變化，而不是關注檔案本身

//.gitignore同樣需要git add

git remote add origin https://github.com/richalso77/GIT_LEARNING.git    //聯接github
git branch -M main
git push -u origin main