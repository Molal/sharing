# Introduction to Python: Open Source IT-USA 
Facilatator: Goerge Migot 
![image](https://user-images.githubusercontent.com/42208250/115008698-1cd5af00-9eb4-11eb-86cc-72722a550acf.png)



Assignment 8 import json, requests data='https://raw.githubusercontent.com/normansimonr/Dumb-Cogs/master/lolz/data/tranzlashun.json' resp=requests.get(data) dictionary=json.loads(resp.text) #print(dictionary)

dictionary = { "Marijuan": "Ndukulu", "Gang": "Geri", "Ciggarrette": "Gife", "Money": "Dache", "Pocket": "Mbosho", "Friend": "Fafiri", "Scavenge": "Hamoch", "Tea": "Icha", "Come": "Kamuthe", "Player": "Lovito", "Rastamen": "Mabingi", "Judge": "Jajiko", "Job": "Jobiso" } word = input("Original word:") if word in dictionary: print("The translation is:", dictionary[word]) else: print("sory, the word has no translation in the dictionary.")

f = open("dictionary", "a") f.write(str({ "Marijuan": "Ndukulu", "Gang": "Geri", "Ciggarrette": "Gife", "Money": "Dache", "Pocket": "Mbosho", "Friend": "Fafiri", "Scavenge": "Hamoch", "Tea": "Icha", "Come": "Kamuthe", "Player": "Lovito", "Rastamen": "Mabingi", "Judge": "Jajiko", "Job": "Jobiso" })) f.close()

#open and read the file after the appending: f = open("dictionary", "r") print(f.read()) f.close()
