import csv
#function for reading csv
def openCSV(fileName):
  fl = open(fileName,'r') #open csv file
  flReader = csv.reader(fl,delimiter=";")
  contents = [] 
  for row in flReader:  #read to 2D list
    contents.append(row)
  print(contents)
openCSV('test.csv')    

