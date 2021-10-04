from requests import post
from time import sleep

while True:
    sleep(0.001)
    json = {'id': 518705815, 'params': "vk_access_token_settings=&vk_app_id=7949771&vk_are_notifications_enabled=1&vk_is_app_user=1&vk_is_favorite=0&vk_language=ru&vk_platform=mobile_web&vk_ref=other&vk_ts=1633269734&vk_user_id=518705815&sign=Ag9b7TLo0vfWGaM0IJPLjeNRt4KBsbvFKIWiJXNiTmo"}
    url2 = 'https://baguette-game.com:2010/buyBoxOne'
    rq2 = post(url=url2, json=json).json()

    trophies = rq2.get("trophies")
    status = rq2.get("status")
    balance = rq2.get("balance")
    earn = (rq2.get("bal"))
    balance_old = balance - earn
    if status == "ok":
        print(f"Успешно купили маленький бокс. Баланс: {earn} Трофеи: {trophies}")
