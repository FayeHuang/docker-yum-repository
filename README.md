# docker-yum-repository
yum repository with tool : createrepo , yum-arch , yum-downloadonly
# 使用方式
將 repository 複製到 /var/www/html 目錄下，build 新的 image，例如 fayehuang/hdp-yum-repository:2.0.0。

或者把 reposiotry mount 到 /var/www/html 目錄下，執行 fayehuang/yum-repository container

  `docker run -d -v /var/www/html:/var/www/html -p 2222:22 -p 8080:80 -e ROOTPASSWORD=<mypassword> fayehuang/yum-repository`
