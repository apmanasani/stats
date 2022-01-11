import numpy as np
from matplotlib import pyplot as plt
from scipy.stats import norm 

print("Select between the following: probability between two values, probability lower than a value, probability higher than a value")
decision = input()

if (decision == "probability lower than a value"):
    ixpoint = 0
    imuinput = 0
    isigmainput = 0

    print("Make sure to use positive numbers for all the values!")
    print("What is the point you are trying to find the z-score for?")
    xpoint = input("point: ")
    ixpoint = float(xpoint)

    print("What is your mean of your normal distribution?")
    muinput = input("mu: ")
    imuinput = float(muinput)

    print("What is your standard deviation of your normal distribution?")
    sigmainput = input("sigma: ")
    isigmainput = float(sigmainput)

    if isigmainput < 0:
        print("ERROR: That isn't a real standard deviation value! Please select a standard deviation that is above 0.")
        print("What is your standard deviation of your normal distribution?")
        sigmainput = input("sigma: ")
        isigmainput = float(sigmainput)

    zsc = (ixpoint - imuinput) / isigmainput
    print("This is your z-score: ", zsc)

    prob = norm(loc = 0 , scale = 1).cdf(zsc)
    print("The probability that the following point or below occurs is: ", prob)

if (decision == "probability higher than a value"):
    ixpoint = 0
    imuinput = 0
    isigmainput = 0

    print("Make sure to use positive numbers for all the values!")
    print("What is the point you are trying to find the z-score for?")
    xpoint = input("point: ")
    ixpoint = float(xpoint)

    print("What is your mean of your normal distribution?")
    muinput = input("mu: ")
    imuinput = float(muinput)

    print("What is your standard deviation of your normal distribution?")
    sigmainput = input("sigma: ")
    isigmainput = float(sigmainput)

    if isigmainput < 0:
        print("ERROR: That isn't a real standard deviation value! Please select a standard deviation that is above 0.")
        print("What is your standard deviation of your normal distribution?")
        sigmainput = input("sigma: ")
        isigmainput = float(sigmainput)

    zsc = (ixpoint - imuinput) / isigmainput
    print("This is your z-score: ", zsc)

    prob = 1 - norm(loc = 0 , scale = 1).cdf(zsc)
    print("The probability that the following point or above occurs is: ", prob)

if (decision == "probability between two values"):
    ixpoint = 0
    ixpoint2 = 0
    imuinput = 0
    isigmainput = 0

    print("Make sure to use positive numbers for all the values!")
    print("What is the first point?")
    xpoint = input("point: ")
    ixpoint = float(xpoint)

    print("What is the second point?")
    xpoint2 = input("point: ")
    ixpoint2 = float(xpoint2)

    print("What is your mean of your normal distribution?")
    muinput = input("mu: ")
    imuinput = float(muinput)

    print("What is your standard deviation of your normal distribution?")
    sigmainput = input("sigma: ")
    isigmainput = float(sigmainput)

    if isigmainput < 0:
        print("ERROR: That isn't a real standard deviation value! Please select a standard deviation that is above 0.")
        print("What is your standard deviation of your normal distribution?")
        sigmainput = input("sigma: ")
        isigmainput = float(sigmainput)

    zsc = (ixpoint - imuinput) / isigmainput
    print("This is your z-score for your first point: ", zsc)

    zsc2 = (ixpoint2 - imuinput) / isigmainput
    print("This is your z-score for your second point: ", zsc2)

    if (zsc2 > zsc):
        prob = (norm(loc = 0, scale = 1).cdf(zsc2)) - (norm(loc = 0 , scale = 1).cdf(zsc))
        print("The probability that a point occurs between these following points is: ", prob)
    elif (zsc > zsc2):
        prob = (norm(loc = 0, scale = 1).cdf(zsc)) - (norm(loc = 0 , scale = 1).cdf(zsc2))
        print("The probability that a point occurs between these following points is: ", prob) 
    elif (zsc == zsc2):
        print("The probability that a point occurs between these following points is: 0")
