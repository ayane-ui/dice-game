# dice-gameimport random

def dice_game():
    name = input("あなたの名前は？\n> ")
    print(f"こんにちは、{name}！\nサイコロを振っています...")

    die1 = random.randint(1, 6)
    die2 = random.randint(1, 6)
    total = die1 + die2

    print(f"サイコロ1: {die1}")
    print(f"サイコロ2: {die2}")
    print(f"合計値: {total}")

    if total > 7:
        print(f"{name} won!")
    else:
        print(f"{name} lost!")

dice_game()
