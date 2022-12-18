# Projektseite "The rise of Grünkohl"



## Konzept
Wir haben uns am Anfang überlegt, ein JumpandRun-Spiel mit Greenfoot zu erstellen.
Dabei sollte es mehrere Level und einen Spieler geben, welcher das Ziel hat, einen Kuchen zu essen.
Dabei soll der Spieler auf dem Weg logischerweise springen müssen, um nicht zu sterben.
Außerdem sollte der Spieler auf dem Weg zum Kuchen Grünkohl und Minze einsammeln können.
Dazu sollte es neben dem Spieler auch andere Actor geben, die sich zum Teil bewegen können, um die Welt etwas lebendiger zu machen.
Wir wollten auch einen Screen dafür, dass der Spieler tot ist und einen dafür, dass er gewonnen hat, wenn er den Kuchen gegessen hat.

## Aufbau
Die Spielfigur, die der Spieler steuert, ist ein Ritter namens Sir Grünkohl.
Dieser hat das Ziel, zum Kuchen zu gelangen und diesen zu verspeisen, um ein Level zu schaffen.
Gesteuert wird er vom Spieler mit den Tasten "A" für links, "D" für rechts und die Leertaste zum Springen.
Dabei darf der Ritter allerdings den Schlangen nicht zu nah kommen, denn sonst töten diese ihn.
Der Ritter muss dabei, um sein Ziel zu erreichen, auch von Plattform zu Plattform springen.
Auf dem Weg zum Kuchen kann er Grünkohl und Minze einsammeln und essen.
Außerdem gibt es in jedem Level einen Frosch, der Fliegen isst, die in der Luft herumfliegen. 
Diese haben aber keinen Einfluss auf den Spieler.
Am Ende ist auf der letzten Plattform jedes Levels ein Kuchen.
Wenn der Ritter diesen isst, gewinnt er das Level und ein "win"-Screen erscheint.
Sollte der Ritter aber davor sterben, erscheint ein "dead"-Screen.


## Die Codes der verschiedenen Klassen/Actors erklärt

### Worlds

#### KnightWorld
Die Welt KnightWorld stellt das erste Level des Spiels dar.

#### KnightWorld2
Die Welt KnightWorld stellt das zweite Level des Spiels dar.

### Actors

#### Fliege
Die Fliege ist ein Actor, der von dem Frosch gegessen werden kann und keinen Einfluss auf den Spieler selber hat.

#### Frosch
Der Frosch ist ein Actor, der Fliegen essen kann. Er kommt einmal in jedem Level vor und hat keinen Einfluss auf den Spieler selber.

#### GameOver
GameOver ist ein Actor, der ausgeführt wird, wenn der Spieler getötet wird. Er bedeckt dann den Bildschirm mit 

#### Grünkohl


#### Infotafel


#### Kuchen


#### Minze


#### Platform


#### Player


#### Player2


#### Schlange


#### Steuerung


#### WinOver
