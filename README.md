# bubble-ogs
get ogs games on bubble
---
take the jsDomloader and paste it into a html element on bubble:
![image](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/7d053a15-bddc-4e2f-bcea-df22aa0ee6b8)

create another html element and paste the bubble-board.html inside it like so.
I used a repeating group but it can be any html element that can create a div.
The data needs to have the type of game (demo, or game) and the id of the OGS game (1234565).
the text inside the div is important so please do not forget it.
![image](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/beceedc6-a72d-4959-8c79-c159df691e11)

once this is set up the jsDomLoader will find all unique gobans.

After this you must set up the custom trigger Run JavaScript:
you must use start(properties) in the script to run the code.
param1 is the board image,
param2 is the black stone image,
param3 is the white stone image.

You can use any image you see fit.
![image](https://github.com/WeiQiPro/bubble-ogs/assets/108106416/273757e5-d716-456f-9461-f0202f223ffd)
