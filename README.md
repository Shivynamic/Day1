# Day1

# BIT MANIPULATION
def getBit(n,pos):
    return ((n&(1<<pos))!=0)
print(int(getBit(4,0)))


def setBit(n,pos):
    return (n|(1<<pos))
print(setBit(5,1))


def clearBit(n,pos):
    return (n & (~(1<<(pos))))
print(clearBit(4,2))


def updateBit(n,pos, value):
    return ((n&(~(1<<pos))) | value<<pos)
print(updateBit(5,1,1))


def checknum(n):
    return ((n&(n-1))==0)

print(checknum(7))
