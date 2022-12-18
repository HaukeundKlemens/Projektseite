# Projektseite "The rise of Grünkohl"



## Konzept
Wir haben uns am Anfang überlegt, ein JumpandRun-Spiel mit Greenfoot zu erstellen.
Dabei sollte es mehrere Level und einen Spieler geben, welcher das Ziel hat, einen Kuchen zu essen.
Dabei soll der Spieler auf dem Weg logischerweise springen müssen, um zu seinem Ziel zu kommen.
Außerdem sollte der Spieler auf dem Weg zum Kuchen Grünkohl und Minze einsammeln bzw. essen können.
Dazu sollte es neben dem Spieler auch andere Actors geben, die sich zum Teil bewegen können, um die Welt etwas lebendiger zu machen.
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
![image](https://user-images.githubusercontent.com/111414678/208299150-b10a35d7-f0fd-482b-a72c-ee2c01a988fa.png)
![image](https://user-images.githubusercontent.com/111414678/208299168-018865e1-8d84-4f0a-b0af-f8ce505cb48d.png)
![image](https://user-images.githubusercontent.com/111414678/208299190-1ce16aef-d0af-456e-b94a-452ae615c6a4.png)

### Actors

#### Fliege
Die Fliege ist ein Actor, der von dem Frosch gegessen werden kann und keinen Einfluss auf den Spieler selber hat.

#### Frosch
Der Frosch ist ein Actor, der Fliegen essen kann. Er kommt einmal in jedem Level vor und hat keinen Einfluss auf den Spieler selber.

#### GameOver
GameOver ist ein Actor, der ausgeführt wird, wenn der Spieler getötet wird. Er bedeckt dann den Bildschirm mit einem "dead"-Schriftzug in rot-schwarzer Farbe. 

#### Grünkohl


#### Infotafel
Auf der Infotafel wird dem Spieler sein Ziel, den Kuchen zu essen mitgeteilt. Sie wurde von uns auf der Seite "pixelart" erstellt und ins Spiel eingefügt. In jedem Level gibt es nahe der Startposition des Spielers eine Infotafel.

#### Kuchen


#### Minze


#### Platform


#### Player


#### Player2


#### Schlange


#### Schlange2


#### Steuerung
Mit der

#### WinOver
WinOver ist ein Actor, der ausgeführt wird, wenn der Actor Kuchen getötet wird bzw., wenn der Spieler den Kuchen isst. Er bedeckt dann den Bildschirm mit einem "win"-Schriftzug in grün-schwarzer Farbe. 
