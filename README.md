# Baseball-league-Entity-Relationship-Diagram-Model
You are hired to create a database for managing the information about a local boy baseball league. This league has more than 20 teams. Each team has a name, base-location (township), and an email address as the contact. Each team has a manager and a coach. Each team has multiple players. A player has a jersey number in his team. But if he plays for another team later, his jersey number may be different. The league needs to keep track all players, including name, phone, DOB, address, and parent’s phone. The information about the game is also important to the league, such as teams played, game time, location and the scores. The league not only wants to know which team plays games, but also which player played at each game and his stats (such as betting statistics, etc.). The coach of team is usually appointed for 2-year term. The league needs to know when a coach is appointed, coach’s contact number, his/her profession, education degree received, etc., A coach may coach different teams at different time period. The information of manager of each team should be also stored in the database, including his/her contact info. A manger may also work for different teams at different time period. Each team has some helpers/assistants who are usually parents or volunteers from local communities. The league also needs to keep track their contact information
<img width="413" alt="Screenshot 2024-03-10 at 5 11 54 PM" src="https://github.com/Fernandezl7/Baseball-league-Entity-Relationship-Diagram-Model/assets/151462732/281551d7-4d80-44cb-bcc8-32e30c398817">

Team(TeamID, name, township, email address)
Player(PlayerID, name, phone_number, DOB, Address, Parents_phone, jersey_number)
Player_Stats(PlayerSID, Games_played, stats)
Games (GameID, Teams_played, game_time, location, scores)
Helper_Assistant(HID, name, phone_number, email address)
Coach(CID, start_term, contact_number, profession, educational_degree)
Manager(MID, Name, Address, email, phone_number)
Plays(PlayerID, TeamID)
Coaches(TeamID,CID)
Manages(TeamID, MID)
Scores(PlayerSID,PlayerID) 
![image](https://github.com/Fernandezl7/Baseball-league-Entity-Relationship-Diagram-Model/assets/151462732/a2fc739f-cb30-4547-a153-175f5e582e2c)
