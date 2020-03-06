def selection():
    selectionNum = int(input("Do you want to order the array in increasing order(1) or decreasing(2)?"))
    if selectionNum == 1 or selectionNum == 2:
        for i in range(len(numList) - 1):
            numInd = i
            for j in range(i + 1, len(numList)):
                if selectionNum == 1:
                    if numList[j] < numList[numInd]:
                        numInd = j
                elif selectionNum == 2:
                    if numList[j] > numList[numInd]:
                        numInd = j
            if numList[i] != numList[numInd]:
                numList[i], numList[numInd] = numList[numInd], numList[i]
    elif selectionNum != 1 or selectionNum != 2:
        print("Please enter a number between 1 or 2.")
        selection()


num = int(input("How many numbers do you want to enter? "))
numList = [int(input("Enter number: ")) for x in range(num)]
print("Unsorted list: ", numList)

selection()

print("Sorted list: ", numList)
