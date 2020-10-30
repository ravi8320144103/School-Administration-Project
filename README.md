# School-Administration-Project
By Ravi Radadiya
import csv

def write info csv(info list):
with open ('student info.csv', 'a', newline'')as csv file:
writer = csv.writer(csv file)

if csv file.tell() == 0:
writer.writerow(["Name", "Age", "Contect Number", "E-mail ID"])

writer.writerow(info list)

if __name__== '__main__':
condition = True
student num = 1

while(condition):
student info = input("Enter student information for student #{} in the following format (Name Age Contect Number E-mail ID):".format(student num)

student info list = student info.split(' ')

print("\nThe entered information is -\nName: {}\nAge: {}\nContect Number:{}\nE-mail ID: {}"
.format(student info list[0]), student info list[1], student info list[2], student info list[3]))

choice check = input("Is the entered information correct? (yes/no): ")

if choice check == "yes":
write info csv(student info list)

condition check = input("Enter (yes/no) if you want to enter information for another student: ")
if condition check == "yes":
condition = True
student num = student num + 1
elif condition check == "no":
condition = False
elif choice check == "no":
print(\nPlease re-enter the value!")
