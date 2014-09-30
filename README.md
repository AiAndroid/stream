#Design for TV metro demo

the Metro style is contructed by two elements:
Album and Display Item

Album can contain multi albums and display items.

Display item can be defined as video, game, app, music and so on.

                Album
                  |
             _____________________________________
             |    ...  |           |       ...    |
           Album      Album    Display Item     Display Item
           
 The main page is defined as Album.
 

![主风格(https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/main.png "应用")

<img src="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/main.png" />

![主风格(https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/main.png "视频")

<img src="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/main.png"/>

##Home JSON definition
<p>
<a href="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/home.json">Home JSON Sample</a>
</p>

##Album
{

    "data": [
        {
            "items": [display items],
            "images": { },
            "name":"应用",
            "times": {
                "updated": 0,
                "created": 0
            },
            "_ui": {
                "type": "metro"
            },
            "id": "recommend",
            "type": "album",
            "ns": "game"
        },
        {
            "items": [display items],
            "images": { },
            "name": "分类",
            "times": {
                "updated": 0,
                "created": 0
            },
            "_ui": {
                "type": "metro"
            },
            "id": "categories",
            "type": "album",
            "ns": "game"
        },
        {
            "items": [dispay items],
            "images": { },
            "name": "视频",
            "times": {
                "updated": 0,
                "created": 0
            },
            "_ui": {
                "type": "metro"
            },
            "id": "recommend",
            "type": "album",
            "ns": "video"
        },
        {
            "items": [display items],
            "images": { },
            "name": "视频分类",
            "times": {
                "updated": 0,
                "created": 0
            },
            "_ui": {
                "type": "metro"
            },
            "id": "categories",
            "type": "album",
            "ns": "video"
        }
    ],
    "preload": {
        "images": []
    },
    "update_time": 0

}

## Display Item
{
    "target": {
        "type": "item"
    },
    "images": {
        "text": {
            "url": "",
            "ani": {},
            "pos": {}
        },
        "icon": {
            "url": "",
            "ani": {},
            "pos": {}
        },
        "back": {
            "url": "http://image.box.xiaomi.com/mfsv2/download/s010/p017VHRusz5g/R2BoGcjC9rNir1.png",
            "ani": {},
            "pos": {}
        },
        "spirit": {
            "url": "",
            "ani": {},
            "pos": {}
        }
    },
    "name": "高德地图",
    "times": {
        "updated": 1404466152,
        "created": 1404454443
    },
    "_ui": {
        "type": "metro_cell_banner",
        "layout": {
            "y": 1,
            "x": 1,
            "w": 1,
            "h": 2
        }
    },
    "id": "180",
    "type": "item",
    "ns": "game"
}


<p>下载测试的APK (download test apk), you can run it at android pad or TV</p>
<a href="https://github.com/AiAndroid/stream/raw/master/tv/game/androidTV.apk">Click Download</a>


