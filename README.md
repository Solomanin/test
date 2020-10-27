# test

name = input("Enter file name: ")
if len(name) < 1 : name = "mbox-short.txt"

fh = open(name)
count = 0
for line in fh:
   if not line.startswith("From:"): continue
           
   word= line.split()
   emil = word[1]
   print(emil)
     

   if line.startswith("From"):
       count = count + 1












print("There were", count, "lines in the file with From as the first word")
