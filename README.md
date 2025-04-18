#Python Project: 
#*Quiz App* 🧠❓

#*Goal* :
#Ask users multiple-choice questions and track their score.

#*Code* :

questions = {
    "What is the capital of France?": "b",
    "Which language is used to write Python?": "a",
    "What does CPU stand for?": "c"
}

options = [
    ["a) Berlin", "b) Paris", "c) Madrid"],
    ["a) Python", "b) HTML", "c) CSS"],
    ["a) Central Programming Unit", "b) Control Panel Unit", "c) Central Processing Unit"]
]

score = 0
for i, question in enumerate(questions):
    print(f"\n{question}")
    for option in options[i]:
        print(option)
    answer = input("Enter your answer (a/b/c): ").lower()
    if answer == questions[question]:
        print("Correct!")
        score += 1
    else:
        print("Wrong!")

print(f"\nYour final score is: {score}/{len(questions)}")


'''*Concepts used*:

- Using dictionaries and lists together

- Looping through structured data

- Accepting user input and comparing answers

- Basic quiz app logic
'''

