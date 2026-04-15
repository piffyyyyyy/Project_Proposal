# Project_Proposal
cs2 aa

import time
nawh = 1
i = 0
inquiry_folder = [1, 2, 3]
municipality_folder = {"Dingaling": "Red", "Cingaling": "Green", "Bingaling": "Yellow"}
while i == 0:
    while nawh == 1:
        print("Options: 1; View All Inquries, 2; Update Municipality Status, 3; EXIT")
        pick = int(input("Please input your option: "))

        if 0 < pick < 3:
            if pick == 1:
                print("Printing Inquires...")
                time.sleep(1)
                for coolio in range(len(inquiry_folder)):
                    time.sleep(1)
                    print(inquiry_folder[coolio])

            elif pick == 2:
                print("Viewing all Municipalities...")
                time.sleep(1)
                for key, value in municipality_folder.items():
                    time.sleep(1)
                    print(f"{key}: {value}")
                print("What status would you like to update?")
                k = 0
                for keys in municipality_folder.items():
                    time.sleep(1)
                    print(f"Type {k + 1} for {keys}")
                    k = k + 1
                pick2 = int(input("Please select your option: "))
                if pick2 == 1:
                    municipality_folder["Dingaling"] = input("Select from Red, Yellow, Green: ")
                elif pick2 == 2:
                    municipality_folder["Cingaling"] = input("Select from Red, Yellow, Green: ")
                elif pick2 == 3:
                    municipality_folder["Bingaling"] = input("Select from Red, Yellow, Green: ")
                print("Displaying all Municipalities Again...")
                for key, value in municipality_folder.items():
                    time.sleep(1)
                    print(f"{key}: {value}")

            print("Sending you back to admin menu....")
        
        elif pick == 3:
            nawh = nawh + 1
        else:
            pick = int(input("Please pick a number from 1 - 4"))
    i = 2
