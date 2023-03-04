# CS-GO-Winner
Predicting the Winner of rounds in GS:GO using Machine Learning.

CS:GO is a tactical shooter, where two teams (CT and Terrorist) play for a best of 30 rounds, with each round being 1 minute and 55 seconds. There are 5 players on each team (10 in total) and the first team to reach 16 rounds wins the game. At the start, one team plays as CT and the other as Terrorist. After 15 rounds played, the teams swap side. There are 7 different maps a game can be played on. You win a round as Terrorist by either planting the bomb and making sure it explodes, or by eliminating the other team. You win a round as CT by either eliminating the other team, or by disarming the bomb, should it have been planted. 


The dataset was originally published by Skybox as part of their CS:GO AI Challenge, running from Spring to Fall 2020.

Variable Definition Key

time_left The time left in the current round.

ct_score The current score of the Counter-Terrorist team.

t_score The current score of the Terrorist team.

map The map the round is being played on. E.g. de_dust2, de_inferno and de_overpass

bomb_planted If the bomb has been planted or not. False = No, True = Yes

ct_health The total health of all Counter-Terrorist players. Player health in range 0-100.

t_health The total health of all Terrorist players. Player health in range 0-100.

ct_armor The total armor of all Counter-Terrorist players.

t_armor The total armor of all Terrorist players.

ct_money The total bankroll of all Counter-Terrorist players. Amount in USD.

t_money The total bankroll of all Terrorist players. Amount in USD.

ct_helmets Number of helmets on the Counter-Terrorist team.

t_helmets Number of helmets on the Terrorist team.

ct_defuse_kits Number of defuse kits on the Counter-Terrorist team.

ct_players_alive Number of alive players on the Counter-Terrorist team. Range 0 to 5.

t_players_alive Number of alive players on the Terrorist team. Range 0 to 5.

ct_weapon_X Weapon X count on Counter-Terrorist team. E.g. Ak47, Deagle and UMP45.

t_weapon_X Weapon X count on Terrorist team. E.g. Ak47, Deagle and UMP45.

ct_grenade_X Grenade X count on Counter-Terrorist team. E.g. HeGrenade, Flashbang.

t_grenade_X Grenade X count on Terrorist team. E.g. HeGrenade, Flashbang.

round_winner Winner. CT = Counter-Terrorist, T = Terrorist




We Perform two maching learning algorithms on the dataset:
1. K Nearest Neighbours
2. Random Forest Classifier

We see that random Forest Classifer performs better than KNN with accuracy of 82% and 78% respectively.

Dataset URL: https://www.openml.org/search?type=data&sort=runs&id=43430&status=active

