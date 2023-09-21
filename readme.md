生成证书

1 安装工具
curl https://get.acme.sh | sh -s email=wuxiu930305@gmail.com

[Thu Sep 21 11:20:11 CST 2023] Installing from online archive.
[Thu Sep 21 11:20:11 CST 2023] Downloading https://github.com/acmesh-official/acme.sh/archive/master.tar.gz
[Thu Sep 21 11:20:14 CST 2023] Extracting master.tar.gz
[Thu Sep 21 11:20:14 CST 2023] It is recommended to install socat first.
[Thu Sep 21 11:20:14 CST 2023] We use socat for standalone server if you use standalone mode.
[Thu Sep 21 11:20:14 CST 2023] If you don't use standalone mode, just ignore this warning.
[Thu Sep 21 11:20:14 CST 2023] Installing to /root/.acme.sh
[Thu Sep 21 11:20:14 CST 2023] Installed to /root/.acme.sh/acme.sh
[Thu Sep 21 11:20:14 CST 2023] Installing alias to '/root/.bashrc'
[Thu Sep 21 11:20:14 CST 2023] OK, Close and reopen your terminal to start using acme.sh
[Thu Sep 21 11:20:14 CST 2023] Installing alias to '/root/.cshrc'
source "/root/.acme.sh/acme.sh.csh"
[Thu Sep 21 11:20:14 CST 2023] Installing alias to '/root/.tcshrc'
source "/root/.acme.sh/acme.sh.csh"
[Thu Sep 21 11:20:15 CST 2023] Installing cron job
26 0 * * * "/root/.acme.sh"/acme.sh --cron --home "/root/.acme.sh" > /dev/null
定时任务
26 0 * * * "/root/.acme.sh"/acme.sh --cron --home "/root/.acme.sh" > /dev/null

. "/root/.acme.sh/acme.sh.env"
[Thu Sep 21 11:20:15 CST 2023] Good, bash is found, so change the shebang to use bash as preferred.
[Thu Sep 21 11:20:16 CST 2023] OK
[Thu Sep 21 11:20:16 CST 2023] Install success!


acme.sh --issue -d bw.jinbei.live --webroot /data/webdev/ssl

-d 域名
-webroot 域名网站根目录