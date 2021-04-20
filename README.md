# travis-
#it is python based project security system

known_users=["Alice","Bob","Claire","Dan","Emma","Fred","Georgie","Harry"]
print(len(known_users))
while True:
    print("hi! my name is travis")
    name=input("what is your name?:").strip().capitalize()

    if name in known_users:
        print("Hello {}!".format(name))
        remove=input("would you like to be removed from the system(Y/N)?:").upper()
        
        if remove == "Y":
            known_users.remove(name)
        elif remove == "n":
            print("No problem,I didn't want you to leave anyway!")
        
    else:
        print("hmm I don't think I have met you yet {}".format(name))
        add_me=input("Would you like to be added to the system(y/n)?:").strip().lower()
        if add_me == "y":
            known_users.append(name)
        elif add_me == "n":
            print("No worries,see you arround!")

