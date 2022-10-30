# BasketMatch
Big Data project from iNeuron

You need to tackle one of the challenges of learning Hadoop, and that's finding data sets that are realistic yet large enough to show the advantages of distributed processing, but small enough for a single developer to tackle. The data set should have play-by-play baseball statistics, available free of charge from Retrosheet. The data is available by year, and includes detailed descriptions of games, plays, and players. This data is especially well-suited for purposes, because a great deal of it is hand-encoded, so there are errors and malformed records that you need to handle.

Each year contains several types of files: Team files, Roster files, and Event files. Team files contain a listing of teams playing each year. Each team listing contains a 3-letter designator that is used to reference that team in all other files. Roster files contain a listing of players for each team, and are named with the 3-letter designator for each team and the year, followed by a .ROS extension. Event files are designated by a .EVA, .EVN, or .EVE extension, depending on whether they are for American League teams (.EVA), National League teams (.EVN), or for post-season games (.EVE). Each event file contains the home games for a single team for a single year. The filename consists of the year included and the 3-letter designator for the home team.

The data is available in gamedata directory.

Since you will have comma-delimited, newline-terminated records, you can use Pig’s built-in PigStorage class to get some more in-depth information about our data set. Let’s start with a few basic questions:

How many games are represented?
How many records do we have total?
What is the relationship between player IDs and player names?
