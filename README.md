#Design for TV metro demo

the Metro style is constructed by two kinds of elements:
Album and Display Item

Album can contain multi albums and display items.

Display item can be defined as video, game, app, music and so on.

You can deprive your own game/app/video detail item from display item.

                Album
                  |
             _____|________________________________
             |    ...  |           |       ...    |
           Album      Album    Display Item     Display Item
           
 The main page is also defined as Album.
 
##API Style
###Details
http://host/game(video/app)/item?id=12346

###Album
http://host/game(video/app)/album?id=6464

###Category
http://host/game(video/app)/category?id=123456
 
##Tab "app/game"(主风格"应用")

<img src="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/en/app_en.png" />

##Tab "video" (主风格"视频")

<img src="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/en/video_en.png"/>

##tab "video category"(主风格"视频分类")

<img src="https://raw.githubusercontent.com/AiAndroid/stream/master/tv/game/en/video_list_en.png"/>

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
            "url": "http://xxx/fffff.png",
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
    


##Download test APK
<p>下载测试的APK (download test apk), you can run it at android pad or TV</p>
<a href="https://github.com/AiAndroid/stream/raw/master/tv/game/androidTV.apk">Click Download</a>

##Welcome to <a href="mailto:liuhuadong78@gmail.com">Contact US<a/>



