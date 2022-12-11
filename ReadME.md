Docker-Cvat安裝過程
======

### Docker部分

+ 首先先安裝Docker

```
https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe

```
![markdown-viewer](image/1.png)

+ 安裝完後重新啟動電腦，再開啟Docker會遇到以下狀況，原因是沒有下載Linux Kernel套件

![markdown-viewer](image/2.png)

+ 點進去網址之後，下載Linux核心套件

![markdown-viewer](image/3.png)

+ 接下來在CMD上輸入指令

```
wsl --set-default-version 2

```

![markdown-viewer](image/4.png)

接下來在Microsoft Store 頁面下載需要的Ubuntu系統，這邊下載20.04版本

![markdown-viewer](image/5.png)

+ 下載完後打開，會需要輸入User Name和Password，這邊就自行輸入需要的，輸入完畢後Windows作業系統就整合Linux發行版本了

![markdown-viewer](image/6.png)

### 安裝git bash

```
https://github.com/git-for-windows/git/releases/download/v2.21.0.windows.1/Git-2.21.0-64-bit.exe

```

+ 基本上直接安裝沒有問題，除非自己有特殊需求在安裝時自行設定，像是在桌面有快捷鍵等等

+ 安裝git bash可以讓你在Github上利用git clone將Github程式碼下載下來

![markdown-viewer](image/7.png)

+ 在安裝完後打開git bash輸入指令將cvat的code下載下來

```

git clone https://github.com/opencv/cvat.git

```

### Cvat下載

+ 從Github上下載完畢後，cd進入cvat

![markdown-viewer](image/8.png)

+ 接下來輸入指令來創建Cvat環境

```
docker-compose up –d

```

+ 若這邊輸入完指令跑出這樣的畫面
