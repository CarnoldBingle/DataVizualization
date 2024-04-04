here is my data vizualization and the code 

import matplotlib.pyplot as plt
import csv

#x = []
#y = []

#with open('crash.csv', 'r') as csvfile:
    #csvplots = csv.reader(csvfile, delimiter=',')

    #for row in csvplots:
        #x.append(row[0].strip('"'))
        #y.append(int(row[1].strip('"')))
        #print(row)

#plt.bar(x, y)
#plt.ylabel("car crashes")
#plt.xlabel("day of the week")
#plt.title("car crashes per day of the week")

#plt.show()

import matplotlib.pyplot as plt
import csv

Names = []
Values = []

with open('NewZealandTemperatures.csv','r') as csvfile:
	lines = csv.reader(csvfile, delimiter=',')
	for row in lines:
		Names.append(row[0])
		Values.append(int(row[1]))

plt.scatter(Names, Values, color = 'g',s = 100)
plt.xticks(rotation = 25)
plt.xlabel('Temp')
plt.ylabel('Year')
plt.title('AverageTemperatureFahr in New Zealand', fontsize = 20)

plt.show()
