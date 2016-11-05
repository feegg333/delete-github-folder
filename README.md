# delete-github-folder

當你想要刪除 GitHub 上的資料夾時，卻發現怎麼也找不到刪除的地方，也不知道從何下手，請參考本篇文章，跟著做就能成功將資料夾刪除啦!


會寫這篇文章是因為以前 GitHub 的版本似乎能夠直接更改資料夾名稱，或是做刪除的動作，但是現在怎麼找卻都找不著在哪邊能夠直接更改，因此使用指令的方式，即可快速地答道我們的目的，將GitHub 上的資料夾刪除。

先來看看 GitHub 上面，為了Demo，先建立了兩個資料夾，分別是 test01 與 test02。

[![ GitHub 上面的檔案](https://dl.dropbox.com/s/fjld77t8bm2kb6y/2016-11-01_01.jpg "GitHub 上面的檔案")](https://dl.dropbox.com/s/fjld77t8bm2kb6y/2016-11-01_01.jpg)

而這次的目標就是要把 test02 這個資料夾刪除。

首先開啟自己習慣的 指令工具，這邊是使用 Git Shell。

打指令前記得先檢查本機路徑是否正確指到要修改的 repository 路徑，確認路徑沒問題以後就可以開始打指令了。


<pre>
C:\github\delete-github-folder [master ≡ +1 ~0 -0 !]>  git rm -r --cached test02
<pre/>


輸入這項指令後，你會看到他已經把該資料夾內的檔案刪除，接著打上 commit。


C:\github\delete-github-folder [master ≡ +0 ~0 -2 | +1 ~0 -0 !]> git commit -m 'remove folder'


最後再使用 push 指令，任務就完成啦!


 C:\github\delete-github-folder [master ↑ +1 ~0 -0 !]> git push origin master


我們到 GitHub 上面看看， test02 資料夾已經成功被刪除了。

[![ test02 資料夾已經被刪除](https://dl.dropbox.com/s/f47j2qjxaicqq69/2016-11-01_02.jpg "test02 資料夾已經被刪除")](https://dl.dropbox.com/s/f47j2qjxaicqq69/2016-11-01_02.jpg)

希望這篇文章可以幫助到想刪除 GitHub 上面的資料夾，卻不知道從何下手的朋友，下台一鞠躬。
