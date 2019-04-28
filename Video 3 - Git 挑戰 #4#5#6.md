# Video 3 - Git 挑戰 456

挑戰 4 - 認識 Github 並註冊 Github 帳號
挑戰 5 - 產生 ssh key 並上傳到 Github，讓 Github 認識你的電腦
挑戰 6 - 將 Repository 推送到 Github 上 

## 挑戰 4 - 認識 Github 並註冊 Github 帳號

認識Github

介紹 Github 與 Git 的差別

![](https://i.imgur.com/0IYv2yn.png)

![](./media/15544860126055/15545652221360.jpg)



## 挑戰 5  - 產生 ssh key 並上傳到 Github 讓 Github 認識你的電腦

## 介紹 ssh 

ssh 分為公鑰和私鑰

- 私鑰儲存在本機電腦中
- 公鑰丟上去服務

當我們要存取服務時，服務會核對公鑰跟我們的私鑰有沒有一致。

![](./media/15544860126055/15545654448968.jpg)


### Windows 

#### 創建 ~/.ssh 資料夾

> `~` 代表使用者目錄

切換到使用者目錄

```
cd ~
```

新增 .ssh 資料夾 

```
mkdir .ssh
```

進入 ~/.ssh 資料

開始產生 ssh key pair


#### 使用 putty 產生 ssh key pair

到 putty 官方網站下載 putty
https://www.putty.org/

使用 putty 產生 ssh key pair
https://www.digitalocean.com/docs/droplets/how-to/add-ssh-keys/create-with-putty/

產生 ssh key 的時候記得要在空白處移動滑鼠。

### Mac

憑證放置位置 

```
cd ~/.ssh
```

如果沒有這個資料夾的話產生一個

```
mkdir .ssh 
```

```
ssh-keygen -t rsa -C "your_email@example.com"
```

金鑰產生的預設位置為 

```
/Users/$YOUR_USER_NAME/.ssh
```

讀取公鑰 
cat id_rsa.pub

![](./media/15544860126055/15545659211856.jpg)




### 產生完 ssh key 後把公鑰上傳到 github 上面

![](https://i.imgur.com/ZlzrPGB.png)

### 在本地端初始化 git 專案

使用 terminal 切換到專案資料夾

```
cd your_project_name 
```

輸入 `git init` 初始化專案，初始化結束後會顯示當下資料夾為 `master` 分支

![](https://i.imgur.com/iK6IfFI.png)


## 建立 github 專案 

![](https://i.imgur.com/FTax5yq.png)

![](https://i.imgur.com/B45texE.png)

![](https://i.imgur.com/qpATONL.png)

![](https://i.imgur.com/JKu2Sxc.png)

選擇使用 ssh 的網址
因為我們已經初始化了 git 專案，所以只要輸入兩個指令即可上傳

![](https://i.imgur.com/4pAc6OT.png)


