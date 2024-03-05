# MDP REPRESENTATION

## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

1.Text representation
2.Graphical representation
3.Python - Dictonary representation

## PROBLEM STATEMENT:

### Problem Description
Consider an AI agent controlling the temperature of a cryogenics lab. The role of the agent is to maintain the lab at a temperature of -5°C

### State Space
{L,E,H} -> {0,1,2}

where,

####      * L -> Lower than expected temperature
####      * E -> Expected temperature
####      * H -> Higher than expected temperature

### Sample State
H -> 2

Higher than expected temperature


### Action Space
{I,D} -> {0,1}

where,

##### I -> Increase the temperature (Using Heater)
##### D -> Decrease the temperature (Using AC)


### Sample Action
I -> 0

##### Increase the temperature (Using Heater)

### Reward Function
```
R = { +1 , if we come closer to the expected temperature
       0 , otherwise
```

### Graphical Representation
![WhatsApp Image 2024-03-05 at 14 38 54_46119bc7](https://github.com/sivabalan28/mdp-representation/assets/113497347/90400c65-89a8-4ebe-ab1e-d8ed9efd6ea1)

## PYTHON REPRESENTATION:
```py
# Creating Dictionary
P = {
    0 : {
        0 : [(1.0, 1, 1.0, True)],
        1 : [(1.0, 0, 0.0, False)]
    },
    1 : {
        0 : [(1.0, 2, 0.0, False)],
        1 : [(1.0, 0, 0.0, False)]
    },
    2 : {
        0 : [(1.0, 2, 0.0, False)],
        1 : [(1.0, 1, 1.0, True)]
    }
}

P
```

## OUTPUT:
![Screenshot 2024-03-05 143447](https://github.com/sivabalan28/mdp-representation/assets/113497347/d82040c1-adae-4f3e-9c09-675f904aa4a7)

## RESULT:
Thus the given Markov Decision Process(MDP) problem is represented in the following ways.

 1.Text representation  
 
 2.Graphical representation 
 
 3.Python - Dictonary representation 
