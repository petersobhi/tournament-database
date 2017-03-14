# tournament-database
Udacity Full Stack Web Developer Nanodegree project

### Requirements

* [Python 2.x](https://www.python.org/)
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)

### Installation
download  or clone the repo:
```sh
$ git clone https://github.com/petersobhi/tournament-database.git
```
move it to the vagrant shared folder and open the SSH session

create the tournament database and import the sql file:
```sh
$ psql
$ create database tournament;
$ \c tournament
$ \a tournament.sql
```
##### now you are ready to use the functions in the ```tournament.py``` module

### Functions
| Function | Description |
| ------ | ------ |
| ```connect()``` | create a connection with the tournament database |
| ```deleteMatches()``` | delete all the matches in the database |
| ```deletePlayers()``` | delete all the palyers in the database |
| ```countPlayers()``` | Returns the number of players currently registered |
| ```countPlayers()``` | Returns the number of players currently registered |
| ```registerPlayer(name)``` | Adds a player to the tournament database with that name |
| ```playerStandings()``` |Returns a list of the players and their win records, sorted by wins |
| ```reportMatch(winner, loser)``` |Records the outcome of a single match between two players |
| ```swissPairings()``` | Returns a list of pairs of players for the next round of a match |

##### there is also a module called ```tournament_test.py``` can be used to test these functions
