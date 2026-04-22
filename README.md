# 📝 Description
Authetication via php
<!--
<table width="100%">
  <tr valign="middle">
    <td align="left">
      <a href="https://github.com/florianthepro/csv-reporting/archive/refs/tags/v1.zip">Sourcecode</a>
    </td>
    <td align="right">
      <a href="https://github.com/florianthepro/csv-reporting/blob/README/01.md">Read →</a>
    </td>
  </tr>
</table>
-->

> [!IMPORTANT]
> pw.txt htaccess sperren

> [!NOTE]
> pw.txt erstellen

> [!TIP]
> Apache+php:
> ```
> sudo apt update \
>&& sudo apt install -y apache2 \
>&& sudo systemctl enable --now apache2 \
>&& sudo apt install -y php libapache2-mod-php php-cli php-common php-mysql php-xml php-curl php-gd php-mbstring \
>&& sudo systemctl reload apache2
> ```
>htaccess nutzen:
> ```
> sudo grep -q "<Directory /var/www/html>" /etc/apache2/apache2.conf || sudo tee -a /etc/apache2/apache2.conf > /dev/null <<'EOF'
><Directory /var/www/html>
>    AllowOverride All
>    Require all granted
></Directory>
>EOF
>sudo apachectl configtest && sudo systemctl reload apache2
>```

Copy paste all to dir

use it (same dir)
```
<?php session_start();require __DIR__ . '/check.php';require_login();?>
```
