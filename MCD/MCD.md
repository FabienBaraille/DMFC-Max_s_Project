Game team, 1N GAME, 0N TEAM
:
GAME:Date and time of Match, Visitor Score, Home Score, Winner, Visitor Odd, Home Odd
:
Contains, 1N ROUND, 11 GAME
:
ROUND: _Name, Category
Play, 0N LEAGUE, 11 ROUND
:
Display, 0N LEAGUE, 11 NEWS
NEWS:_title, description

:
:
:
Contains 2, 11 TOP1O, 1N ROUND
:
:
:

TEAM:Trigram, Name, Conference, Logo, Ranking
Participate, 0N TEAM, 1N TOP1O
:
:
TOP1O:Conference, deadline, results
:
Create, 0N USER, 11 ROUND
Has, 1N SEASON, 11 ROUND
SEASON:Year, Start season, Start playoff
:
LEAGUE:League name, League description

:
:
SR PREDICTION, 0N USER, 0N GAME:Predicted winning team, Predicted point difference, Validation status (saved, validated, published), Point scored, Bonus points earned, Bonus Bookie
:
Bet, 0N USER, 0N TOP1O: predicted ranking, validation status, points earned
:
:
Leaderboard, 0N SEASON, 0N USER: Final score, Final rank
:
Belong to, 11 USER, 1N LEAGUE
:
:

:
Love, 01 USER, 0N TEAM
:
:
:
:
USER:Username, Password (encrypted), Email, Role, Title, Score, Old position, Season played
:
:
:
:

:
:
:
:
request, 0N USER, 11 RESET PASSWORD REQUEST
RESET PASSWORD REQUEST:_Selector, Hashed token, Requested at, Expires at

:

:
select, 1N TEAM, 1N LEAGUE:Selected Away, Selected Home
