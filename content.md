### izveidot number guessing spēli ar python programēšanas valodu

### saturs

### 1.aprakstīt spēli
### 2.spēles loģika

```py

import random

repeat = True

while repeat:
    number = random.randint(1, 100)
    guess = 0
    tries = 0

    while guess != number:
        if guess < number:
            print("Pamēģini leilāku skaitli.")
        else:
            print("Pamēģini mazāku skaitli.")

        guess = int(input("Uzmini skaitli: "))
        tries += 1
    else:
        if tries < 4:
            print(f"WOW! uzminēji tikai pēc {tries} reizēm!")
        elif tries < 7:
            print(f"Nav slikti, uzminēji pēc {tries} reizēm!")
        else:
            print(f"Hm... vajadzētu patrenēties, uzminēji pēc {tries} reizēm!")

    response = input("Vai gribi turpināt? y/n: ")    
    if response == "y":
        repeat = True
    elif response == "n":
        repeat = False
        print("Paldies par spēli! Bye, bye!")
    else:
        repeat = False
        print("Paldies par spēli!  Bye, bye!")


```
### 3.
