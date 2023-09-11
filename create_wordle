import random

def give_instructions():
    print('''Wordle is a word guessing game.
    You have 5 attempts
    (✅) means the letter is in the correct position.
    (😙) means the letter is in the word but not in the right position.
    (😒) means the letter is not in the word at all. 

    Best of Luck :)
    ''')

words = ["pink", "this", "that", "cats", "five", "word", "lake"]

hidden_word = random.choice(words)


def check_word(guess):
    if hidden_word == guess:
        print("Congrats!!! You did it.")
        return True
    else: 
        result = ""
        for i,j in zip(guess, hidden_word):
            if i == j:
                result = result + "(✅)"
            elif i in hidden_word:  
                result = result + "(😙)"
            else: 
                result = result + "(😒)"
        print(result)
        return False
    
def main():
    give_instructions()
    attempt = 5
    while attempt>0:
        guess = input("enter a four letter word:  ")
        if check_word(guess):
            break
        else:
            attempt -= 1
            print(f"You have {attempt} attempts left.")
    else:
        print("GAME OVER")
 



main()
