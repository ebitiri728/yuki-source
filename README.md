# Summary / 概要
Yuki Youtubeに機能を追加します。<br>
随時アップデート中につきバグ等発生の可能性あり。


# How to Use / 追加方法
BBS:<br>
    main.pyに<br>
    ```
    @cache(seconds=60)
    def getSource(name):
        return requests.get(f'https://raw.githubusercontent.com/LunaKamituki/yuki-source/main/{name}.html').text
    ```<br>
    を追加し、/bbsと/bbs/resultに
    ```.return ~~~y)}", cookies={"yuki":"True"})```<br>
    の後に
    ```.text.replace('AutoLink(xhr.responseText);', 'urlConvertToLink(xhr.responseText);') + getSource('bbs')```
    と追加する。
