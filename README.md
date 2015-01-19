# LichessTV Embedder

Chrome extension that allows you to embed draggable LichessTV http://en.lichess.org/tv
onto the webpage of your choice. Uses draggable.js https://github.com/gtramontina/draggable.js.

![Demo](https://s3.amazonaws.com/f.cl.ly/items/103Y3g2P0U3s2k1L0C1G/Screen%20Recording%202015-01-18%20at%2008.29%20PM.gif)

## Setting Up

1. Download and open the ZIP file.
2. Type chrome://extensions/ in the address bar.
3. Check "Developer mode" on the top right.
4. Click "Load unpacked extension."
5. Select the folder that contains downloaded files.
6. Go to [Niconico](http://www.nicovideo.jp/) or [twitch](http://www.twitch.tv/) and see what happens!

## Customization

1. Open manifest.json
2. Take a look at this [guide](https://developer.chrome.com/extensions/content_scripts), and change the "matches" property on "content_scripts."
3. Examples:
    * use /<all_urls> to embed LichessTV on all websites you visit.
    * "matches": ["http://shinuesugi.com/"] embeds LichessTV when visiting my website.
    * "matches": ["http://nicovideo.jp/*"] embeds LichessTV on any websites that start with http://nicovideo.jp/, but will not include websites such as http://live.nicovideo.jp/.
