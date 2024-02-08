# Seaborn_HW

import pandas as pd

p=pd.read_csv("pokemon.csv")

team=[]

#pandas check for specific input being present or not
#p.loc[p['identifier']=='bulbasaur'].empty

while True:
    n=input("What would you like to do:\n\n\t1) Add teammate\n\t2) Exit\n\t3) manage: Team\n\n\input: n=input("Generate your own team\n\t4")")
    if int(n)==1:
        t=input("Who is your teamate: ")
        if len(team) == 3:
            print("Too many teammates")
            continue
        elif p.loc[p['identifier']==t].empty:
            print("Invalid Pokemon")
            continue
        team.append(t)
        print(team)
        #print(len(team))
    if int(n)==3:
        p=input("what would you like to do:\n\nt3) Change")
    if int(n)==2:
        # print("change")
        team.sort(reverse=True)
        old=team.index("squirtle")
        e=team.pop(old)
        print(e)
        team.insert(2,e)
        print(team.sort())
    if int(n)==2:
        print("world")
        break
print(pokemon.csv)
print(teams)

if bulbasar < 6 : 
    print("too many in the list")

if squirtle > 6 : 
    print("list needs widened")

# These should show how the teams have been rearranged. 

pokemonvariables = dict(pokemon.csv)
squirtlevariables = dict(pokemon.csv)

bulbasarvariables.update(id=6,name="bulbasa variables")
squirtlevariables.update(id=6,name = "squirtle variables")
