# python-basics-basics 
""" s = "Hello Python"
print(s)      # prints whole string
print(s[0])   # prints "H"
print(s[1]) # prints "e" 
 print(" shift+alt+A ")
print("comment out") 
 age = 24 
print("guess  my age you have 1 chance  ")
guess = int(raw_input("guess:"))
if guess!= age:
    print("wrong!")
else:
    print("correct")  """  

# # a few ways to do this
# print("subscribe to " + youtuber)
# print("subscribe to {}".format(youtuber))
# print(f"subscribe to {youtuber}")
"""adj = input("Adjective: ")
verb1 = input("Verb: ")
verb2 = input("Verb: ")
famous_person = input("Famous person: ")

madlib = f"Computer programming is so {adj}! It makes me so excited all the time because \
I love to {verb1}. Stay hydrated and {verb2} like you are {famous_person}!"

print(madlib) 
# guessing game
import random 
def guess (x):
    random_number = random.randint(1,x)
    #print (random_number)
    guess =0
    while  guess!= random_number:
            guess=int(input(f"enter the guess number between 1,{x} : "))
            if guess < random_number:
                print("guess a little higher ") 
            elif guess> random_number:
                print("sorry, guess again little lower")
            else:
                 print(f"yay you get it the correct number is indeed {random_number } ")    
       
guess(10)
name =' '
while name  !='shlok':
    name =input("enter the name : ")
    if name !='shlok':
       i=input("sorry type again sir press ENTER ")
    else:  
        print ("thank you sir")  
while True:
    print('Who are you?')
    name = input()
    if name != 'Joe':
       continue
    print('Hello, Joe. What is the password? (It is a fish.)')
    password = input()
    if password == 'swordfish':
      break
print('Access granted.')
print("my name is ")
for i in range(5):
    print(f"jimmy five times {i}")"""
import random
# library that we use in order to choose
# on random words from a list of words

name = input("What is your name? ")

# Here the user is asked to enter the name first

print("Good Luck ! ", name)

words = ['rainbow', 'computer', 'science', 'programming',
		'python', 'mathematics', 'player', 'condition',
		'reverse', 'water', 'board', 'geeks']

# Function will choose one random
# word from this list of words
word = random.choice(words)


print("Guess the characters")

guesses = ''

# any number of turns can be used here
turns = 12


while turns > 0:

	# counts the number of times a user fails
	failed = 0

	# all characters from the input
	# word taking one at a time.
	for char in word:

		# comparing that character with
		# the character in guesses
		if char in guesses:
			print(char, end=" ")

		else:
			print("_")

			# for every failure 1 will be
			# incremented in failure
			failed += 1

	if failed == 0:
		# user will win the game if failure is 0
		# and 'You Win' will be given as output
		print("You Win")

		# this print the correct word
		print("The word is: ", word)
		break

	# if user has input the wrong alphabet then
	# it will ask user to enter another alphabet
	print()
	guess = input("guess a character:")

	# every input character will be stored in guesses
	guesses += guess

	# check input with the character in word
	if guess not in word:

		turns -= 1

		# if the character doesn’t match the word
		# then “Wrong” will be given as output
		print("Wrong")

		# this will print the number of
		# turns left for the user
		print("You have", + turns, 'more guesses')

		if turns == 0:
			print("You Loose")

print ( "word is : ",word)
  
    

