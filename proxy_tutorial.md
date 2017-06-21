Why proxy ?
------------

Because proxy may help us bypass blocking of some websites, this could help us
increase the success rate to download the images.

How to setup proxy?
------------

1. Click the Settings button.![pic_00](
https://s22.postimg.org/r4eyxe775/setting_button.png
)
1. Select Proxy![pic_01](
https://s16.postimg.org/amzdag0lx/proxy_00.png
)
1. Select the modes(No proxy, Manual proxy, Tor proxy)




No proxy
------------

This mode do not use any proxy and is the default mode

Manual proxy
------------

This mode allow you to setup multiple proxies at once, when the QImageScraper failed to download
full size image, it will instead download the images in the proxy list with random order.

### Setup

1. Select manual proxy
1. Press add button![pic_02](https://s12.postimg.org/ms1gpekkt/proxy_01.png)
1. Enter host, port, user name(optional), password(optional) and type of your proxies

### Type of proxy

- DefaultProxy : Proxy is determined based on the application proxy
- Socks5Proxy : Socks5 proxying is used
- HttpProxy : HTTP transparent proxying is used
- HttpCachingProxy : Proxying for HTTP requests only
- FtpCachingProxy : Proxying for FTP requests only

Tor proxy
------------

[Tor](https://www.torproject.org/) is free software for enabling anonymous communication, with this powerful 
browser, we can easily change our ip address from time to time. If you select to use tor proxy mode, 
QImageScraper will download the images by Tor network if it failed to download full size image.

### Setup Tor

1. [Download Tor](https://www.torproject.org/download/download-easy.html.en)
1. Extract Tor
1. Go to your_path/tor-browser/Browser/TorBrowser/Data/Tor/
1. Open torrc
1. Add hash code as following shown(cautious, you need to hash the passwords by yourself)![pic_02](https://s11.postimg.org/5jhqx0l4z/proxy_02.png)

### How to generate hash password

1. If you are using linux, enter "sudo apt-get update && sudo apt-get install tor"
1. After that, enter "tor --hash-password your_password"
1. copy the password generated by tor to torrc

### Setup tor configuration on QImageScraper

1. Select Tor proxy
1. Enter data of Tor, they are port, control port, host and password. Except of password, everything exist default value
1. Click "Test for validation"![pic_03](https://s8.postimg.org/57trpvho5/proxy_03.png)
1. If everything are fine, you will see a message box pop up and said "You are good to go", else you will error messages