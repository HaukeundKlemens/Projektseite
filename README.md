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
![image](https://user-images.githubusercontent.com/111414678/208299245-32a5d327-f974-44c2-9273-8805382d0270.png)
![image](https://user-images.githubusercontent.com/111414678/208299264-47000b70-3aad-41a6-96e1-04e5d2b4d0bd.png)

### Actors

#### Fliege
Die Fliege ist ein Actor, der von dem Frosch gegessen werden kann und keinen Einfluss auf den Spieler selber hat.
![image](https://user-images.githubusercontent.com/111414678/208299397-221cfde1-1a86-4625-9def-851f85242708.png)


#### Frosch
Der Frosch ist ein Actor, der Fliegen essen kann. Er kommt einmal in jedem Level vor und hat keinen Einfluss auf den Spieler selber.
![image](https://user-images.githubusercontent.com/111414678/208299427-162e34a7-fc19-4e7c-9dc9-fd29c06e336b.png)
![image](https://user-images.githubusercontent.com/111414678/208299440-5057b6fb-7cf5-48ef-953b-e863b20ce4ba.png)
![image](https://user-images.githubusercontent.com/111414678/208299531-152c0bee-a59e-4d93-ae85-9f57e12dd6d8.png)
![image](https://user-images.githubusercontent.com/111414678/208299539-7aca42f9-a294-440f-8dd2-96db05aa8722.png)



#### GameOver
GameOver ist ein Actor, der ausgeführt wird, wenn der Spieler getötet wird. Er bedeckt dann den Bildschirm mit einem "dead"-Schriftzug in rot-schwarzer Farbe. 
![image](https://user-images.githubusercontent.com/111414678/208299554-0970a94d-2e1a-4d37-87f7-f29adfd78b7e.png)


#### Grünkohl
![image](https://user-images.githubusercontent.com/111414678/208299568-7e2692e4-778f-40be-8270-af50950889ba.png)


#### Infotafel
Auf der Infotafel wird dem Spieler sein Ziel, den Kuchen zu essen mitgeteilt. Sie wurde von uns auf der Seite "pixelart" erstellt und ins Spiel eingefügt. In jedem Level gibt es nahe der Startposition des Spielers eine Infotafel.
![image](https://user-images.githubusercontent.com/111414678/208299587-12127aae-48ed-4926-ac6d-5a3043662fd0.png)


#### Kuchen


#### Minze
![image](https://user-images.githubusercontent.com/111414678/208299622-46b6cfd8-d089-49e9-b28a-1323c6c448cc.png)



#### Platform
![image](https://user-images.githubusercontent.com/111414678/208299639-2ec66d0e-f069-466c-a8fa-64fb63dcc9c9.png)



#### Player
![image](https://user-images.githubusercontent.com/111414678/208299750-58f584b4-1cc0-4889-a5b9-0023ecbbc46f.png)
![image](https://user-images.githubusercontent.com/111414678/208299774-e0fc016c-5dd1-458c-93cd-9f95523ceab7.png)
![image](https://user-images.githubusercontent.com/111414678/208299786-12bca19b-e778-4fc3-bebc-8d8104e14221.png)
![image](https://user-images.githubusercontent.com/111414678/208299803-347105f4-9751-4529-9991-14bb1696df53.png)
![image](https://user-images.githubusercontent.com/111414678/208299843-61c2c22e-3966-4b96-94d3-4c367d2d8bc7.png)



#### Player2
![image](https://user-images.githubusercontent.com/111414678/208300406-06cf85c6-ef02-4de2-ad14-854704a31952.png)
![image](https://user-images.githubusercontent.com/111414678/208300429-e8006e79-4ae1-46ed-977e-55e1fb457f2f.png)
![image](https://user-images.githubusercontent.com/111414678/208300447-35fa586c-3928-4579-9672-60e069391255.png)
![image](https://user-images.githubusercontent.com/111414678/208300466-fdf23c41-e9e8-4f8d-a8d7-60ad9c4a327e.png)



#### Schlange


#### Schlange2


#### Steuerung
Mit der

#### WinOver
WinOver ist ein Actor, der ausgeführt wird, wenn der Actor Kuchen getötet wird bzw., wenn der Spieler den Kuchen isst. Er bedeckt dann den Bildschirm mit einem "win"-Schriftzug in grün-schwarzer Farbe. 
