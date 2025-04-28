# Описание
Вирус [free-robux.rar](https://github.com/PykitYT/Virus/blob/main/free-robux.rar)  не навредит вашему компютеру, его можно использавать для пранков.

main.exe - прога которая запускает

остальное - вирусы
Что делает вирус:
+ Через 5 секунд откривает 2 рандомных проги
+ ```
  import os
  import time
  import random
  import threading
  import keyboard as key
    
  run = True
  slc = ["HACKED_BIOS.exe", "spam.exe"]

  def loop():
    global run
    while run:
        r(random.choice(slc))
        time.sleep(5)

  def r(name):
    os.system(name)
    print('Ended.')

  def reset():
    global run
    run = False
    time.sleep(0.1)  # чуть подождать, чтобы старый цикл завершился
    run = True
    threading.Thread(target=loop).start()

  # Горячая клавиша на Enter
  key.add_hotkey("enter", reset)

  # Запускаем основной цикл в потоке
  threading.Thread(target=loop).start()

  # Чтобы программа не завершалась
  key.wait()
+ Рандомные штуки: фейк биос ошибка, спам cmd
# что делать если вирус начинает спамить cmd.exe?

  Нажмите пробел, тогда оно закроет
  
  Если не работает, побробуйте ещё раз.
  
  Бывает баг что оно сразу много вирусов откривает
