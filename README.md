# NewAI

print("Я загадал число от 1 до 100. Попробуй угадать!")

while True:
    try:
        guess = int(input("Введи число: "))
        attempts += 1
        
        if guess < number:
            print("Загаданное число больше.")
        elif guess > number:
            print("Загаданное число меньше.")
        else:
            print(f"Поздравляю! Ты угадал число {number} за {attempts} попыток.")
            break
    except ValueError:
        print("Пожалуйста, вводи только числа.")
