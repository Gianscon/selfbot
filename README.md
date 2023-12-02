#Selfbot Việt Hóa By Zin
## 👑・ Tính Lăng

-   Tự Hunt
-   Tự Battle
-   Inventory Check
    -   Tự dùng Gem ( Trừ Legendary và Mythic )
    -   Tự dùng Lootbox và Fabled Lootbox
    -   Tự dùng Crate
    -   Tự dùng hộp Event ( Lúc có lúc không )
-   Tự đánh bạc ( Tỉ lệ win 80% nếu auto )
    -   Tự Cf ( Coinflip )
    -   Tự S ( Slots )
-   Tự Sell Animals trong Zoo hoặc Sac,
-   Tự update Autohunt
-   Tự Pray
-   Tự làm Checklist
    -   Tự làm quest
    -   Tự nhận quà hàng ngày
    -   Tự gửi Cookie ( Tạm thời dừng hoạt động vì gây BAN tạm thời )
-   Tự kiểm tra Captcha ( Độ chính xác khá kém )
-   Có Discord RPC
-   **Extra Token**
    -   Tất cả các tính năng của Main Token ( Bên trên )
    -   Tự Pray cho Main

## ⚙・Ví dụ cho config.json

```
{
    "settings": {
        "huntandbattle": "", true hoặc false
        "banbypass": "", true hoặc false
        "discordrpc": "", true hoặc false
        "pray": "", true hoặc false
        "extratoken": "", true hoặc false
        "autoquest": "", true hoặc false
        "inventory": {
            "inventorycheck": "", true hoặc false
            "gemcheck": "", true hoặc false
            "lootboxcheck": "", true hoặc false
            "fabledlootboxcheck": "", true hoặc false
            "cratecheck": "", true hoặc false
            "eventcheck": "" true hoặc false
        },
        "animals": {
            "enable": "", true hoặc false
            "type": "" sell hoặc sacrifice
            "ifsacrifice": {
                "common": "", true hoặc false
                "uncommon": "", true hoặc false
                "rare": "", true hoặc false
                "epic": "", true hoặc false
                "mythical": "", true hoặc false
                "patreon": "", true hoặc false
                "cpatreon": "", true hoặc false
                "legendary": "", true hoặc false
                "gem": "", true hoặc false
                "bot": "", true hoặc false
                "distorted": "", true hoặc false
                "fabled": "", true hoặc false
                "special": "", true hoặc false
                "hidden": "" true hoặc false
                "all": "",true hoặc false , nếu true thì tất cả cái bên trên để false
            }
        },
        "upgradeautohunt": {
            "enable": "", true hoặc false
            "type": "" efficiency, duration, cost, gain, exp hoặc radar
        },
        "gamble": {
            "coinflip": {
                "enable": "", true hoặc false
                "amount": "1" Số lượng Cowoncy muốn cá cược
            },
            "slots": {
                "enable": "", true hoặc false
                "amount": "1" Số lượng Cowoncy muốn cá cược
            }
        }
    },
    "main":{
        "token":"", main token (Nếu dùng replit thì chỉnh sửa .env file)
        "userid":"", token user id
        "channelid":"", channel id for main token
        "owodmchannelid":"", owo bot dm channel id
        "autoquestchannelid":"" auto quest channel id | Recommend để id cùng với channelid cho dễ quản lý
    },
    "extra":{
        "token":"", extra token (Nếu dùng replit thì chỉnh sửa .env file)
        "userid":"", extra token user id
        "channelid":"", channel id for extra token
        "owodmchannelid":"" extra token owo bot dm channel id 
        "autoquestchannelid":"" auto quest channel id | Recommend để id cùng với channelid cho dễ quản lý
    }
}
