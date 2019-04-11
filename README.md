# Poker and Maze games using Reinforcement Learning

• Q-Learning algorithm to implement maze and poker problems in reinforcement learning.
• Implemented MazeAgent and PokerAgent to learn based on rewards using Q-Learning methodology.
• Q-Learning is off-policy that learns values based on action obtained from another policy. 
• In Q-Learning approach, current state values are updated based on max rewards action in next state.

Description of maze problem:
A maze is a collection of paths from starting point to goal. Our aim is to start at a valid point in maze and move towards goal point through a valid path. Valid path should include only blocks through which we can move such as open space. Any blocks such as wall or obstacles in path is not a valid one.

Our maze environment is a 2 dimensional matrix with blocks of 'O'(open space), 'H'(Wall or obstacles) and 'G'(Goal location). Our path should have all 'O' blocks to reach goal 'G'. Using Reinforcement Learning, we generate possible paths from every point in maze to reach goal.


Description of poker problem:
Poker is a one card game played among 2 or more players with an objective to empty other players bet amount. Unique cards in this game are 1 to 13. There are a total of 2 rounds where each player can bet 0,1,2,3 with repect to current state of game. Each player starts game with a bet of 1. In round 1, if a player bets more than other players, only other players get chance to either match the bet or fold the game in round 2. In round 2, if bet is matched, cards are revealed and the player with maximum value card wins the game and total bet amount. If bet is not matched in round 2, player with highest bet amount wins the game and total bet amount. Game is continued until a player wins all other players bet amount.

In a game between 2 players each player starts game with his share of 10 and bets 1 before starting. Each player gets a card randomly and doesn't show it to others. In round 1 , players 1 bets 3 for his card numbered 10 and player 2 bets 2 for his card numbered 8. In round 2, player 2 has one more chance to either raise his bet or fold the game(0). Now player 2 raises bet by 1 to a total of 3. The total bet amount in pot is 8(1+1+3+2+1). Both players reveal their cards, player 1 wins the game with a reward of 8(total in pot). This is continued until one player has no more amount to play the game.


