8th april
# Plan:
Make a casino with 3 games, Blackjack, Roulette and Slots, Recording 
online gaming!!!!
## Player data
	Required Database tables:
		Player Saved data
			Player ID
			Player Name
			Player Password
			Player Total Winnings / Losses
			Game History
				Last Game ID (Which game they had in progress)
					Last Bet
						Roulette Current Ws/Ls
							Current placed bets
							
						Blackjack Current Ws/Ls
							Current hand
						Slots Current Ws/Ls
				
				Cashed out?
			

| Player Data   | Data Type |
| ------------- | --------- |
| PlayerID      | PK int    |
| Name          | str       |
| Password      | str       |
| TotalWinnings | int       |
| LastGameID    | FK int    |
| LastGState    | obj       |


| Game Data | Data Type |
| --------- | --------- |
| GameID    | PK int    |
| GameType  | int       |
## Blackjack Data Table


| Blackjack | Data Type |
| --------- | --------- |
| GameID    | PK int    |
| HandID    | int       |
| DHandID   | int       |
| BJBetID   | int       |
| PlayerID  | FK int    |

| BJBet Table | Data Type |
| ----------- | --------- |
| BJBetID     | PK int    |
| BetAmount   | int       |
| SB213       | int       |
| SBPairs     | int       |

## Roulette Data Table 


| Rouletete | Data type |
| --------- | --------- |
| GameID    | PK int    |
| Result    | int       |



| RBet Table  | Data Type |
| ----------- | --------- |
| BetID       | PK int    |
| PlayerID    | FK int    |
| BetPosition | int       |
| GameID      | FK int    |
|             |           |
betposition : assign value to each position 0-36 + values for 3:1 and 2:1's , if bet made is on multiple store both???

## Slots Data Table

| Slots     | Data Type |
| --------- | --------- |
| GameID    | PK int    |
| BetAmount | int       |
| Result    | int       |
| PlayerID  | FK int    |

Odds : Multipliers
Cherry x2 bet if 1 is present, x5 if 2 are present, x8 if 3 are
lemon x 3 if all 5
orange x 4 if all 6 
plum x 5 if all 7
bell x 6 if all 8
bar x 7 if all 9 
7 x 10 if all 10

## Casino Main
	Systems:
		Ask for login
		Menu with game options 
		
  
## Blackjack
	Systems:
		Place bet
		Deal Cards 
		Double Down
		Offer Hit / Stand / Split if avaliable
		If hit, hit till stand / bust
		If split Offer hit or stand on card 1
		If hit, hit till stand / bust
		Repeat for card 2
		Result
		Game Restarts
		Offer rebet / double and play 

## Roulette
	Systems:
		Place bets
		Spin
		Result
		Game Restarts
		Offer rebet / double and play

## Slots 
	Systems:
		Place bet
		Spin
		Result
		


# [[Report]]

### Structure
1. **Title Page:**
    
    - Title of the project
    - Author(s) name
    - Date of completion
2. **Abstract:**
    
    - Brief overview of the project objectives
    - Summary of the methods used
    - Key findings or conclusions
3. **Section 1: Introduction**
    
    - Brief introduction to the project
    - Description of the small casino game
    - Explanation of the purpose and scope of the project
4. **Section 2: Aims and Objectives**
    
    - Summary paragraph outlining the objectives
    - Bullet-pointed list of overall aims
5. **Section 3: Method**
    
    - Description of the development process
    - Explanation of the technologies used (e.g., Python, libraries)
    - Overview of the game design and implementation
6. **Section 4: Results and Discussion**
    
    - Presentation of the final game
    - Screenshots of the game interface
    - Discussion of successful aspects and challenges faced
    - Analysis of player interactions and simulated casino experience
7. **Section 5: Conclusion and Further Work**
    
    - Summary of the project outcomes
    - Lessons learned from the development process
    - Suggestions for future improvements or enhancements
    - Additional features or functionalities for further development
8. **References**
    
    - List of references cited in the report (Harvard format)
9. **Appendices** (if necessary)
    
    - Additional supporting materials such as code snippets, diagrams, or documentation
