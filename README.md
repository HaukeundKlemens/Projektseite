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

## Start und Ende

Vor dem Start kann man sich zwischen zwei Leveln entscheiden, dies kann man rechts oben im Menü machen, danach kann man auf "run" klicken und das Spiel startet.
Das Spiel kann mit dem Tod durch die Schlange, oder dem Erreichen des Kuchens, beendet werden.

## Die verschiedenen Klassen/Actors erklärt

### Worlds

#### KnightWorld
Die Welt KnightWorld stellt das erste Level des Spiels dar.
![image](https://user-images.githubusercontent.com/111414678/208318202-5bbf5af2-28b8-403d-917a-ca7ab4bfd00e.png)
Der Code beginnt mit zwei Variablen, die im Code erklärt sind.
In public KnightWorld() wird zuerst die Fenstergröße gewählt, die Super, das false hebt die Seitenbeschränkung für das Bild auf.
Darunter wird der Hintergrund ausgewählt und platziert.
fillWorld() und prepare() sind beide dazu da, objekte in der Welt zu platzieren.
Die act() Methode aktualisiert jeden Tick die Position der Welt, da drawBackground(), was dort ausgeführt wird dort aktiviert ist.
Die fillWorld Methode fügt der Spieler hinzu.
![image](https://user-images.githubusercontent.com/111414678/208318232-d766fec1-1353-47dc-a6a9-c941f859026d.png)
Die changeBackground(int changeX) Methode greift auf die Variable für den Hintergrund zu, dann wird die Ursprungskoordinate genommen und um die Veränderung durch die Bewegung berechnet.
in der drawBackground() Methode wird dann noch der Hintergrund dieser Veränderung angepasst.
![image](https://user-images.githubusercontent.com/111414678/208318250-4a735a19-bbd7-47d6-9626-050a4614d5c6.png)
![image](https://user-images.githubusercontent.com/111414678/208318265-efd854f7-abd7-4d32-95af-23009118479e.png)
![image](https://user-images.githubusercontent.com/111414678/208318281-26b8b30e-46c2-47d1-9a91-9247aa097b69.png)
Die Methode prepare setzt die verschiedenen Aktoren, die gelistet sind in die Welt, wir haben diese dann noch ein wenig aufgeräumt.
Das einfügen von für den Spieler harmlosen Schlangen in die Welt ist geplant.



#### KnightWorld2
Die Welt KnightWorld2 stellt das zweite Level des Spiels dar. Hier gibt es keine große Änderung zum anderen Level, außer, dass der Actor hier Player2 und nicht Player heißt und das Level anders aufgebaut ist.
![image](https://user-images.githubusercontent.com/111414678/208299150-b10a35d7-f0fd-482b-a72c-ee2c01a988fa.png)
![image](https://user-images.githubusercontent.com/111414678/208299168-018865e1-8d84-4f0a-b0af-f8ce505cb48d.png)
![image](https://user-images.githubusercontent.com/111414678/208299190-1ce16aef-d0af-456e-b94a-452ae615c6a4.png)
![image](https://user-images.githubusercontent.com/111414678/208299245-32a5d327-f974-44c2-9273-8805382d0270.png)
![image](https://user-images.githubusercontent.com/111414678/208299264-47000b70-3aad-41a6-96e1-04e5d2b4d0bd.png)

### Actors

#### Fliege
Die Fliege ist ein Actor, der von dem Frosch gegessen werden kann und keinen Einfluss auf den Spieler selber hat.
![image](https://user-images.githubusercontent.com/111414678/208299397-221cfde1-1a86-4625-9def-851f85242708.png)
Die Fliege hat nur den act() Befehl und dieser gibt der Fliege nur die ständige Veränderung ihrer Flugbahn in einem maximal 45 Grad Winkel vor, dieseVeränderung wird durch einen Zufallsgenerator bestimmt.
Wenn sie sich am Rand Befindet dreht sie sich um  180 Grad.
Außerdem sind darunter zwei Möglichkeiten, die Fliege zu bewegen gelistet, welche allerdings inaktiv sind. 

#### Frosch
Der Frosch ist ein Actor, der Fliegen essen kann. Er kommt einmal in jedem Level vor und hat keinen Einfluss auf den Spieler selber.
![image](https://user-images.githubusercontent.com/111414678/208299427-162e34a7-fc19-4e7c-9dc9-fd29c06e336b.png)
VerticalSpeed ist eine Variable. Die act() Methode lässt die Codes immer wieder ausführen. Der Befehl MoveAndTurn lässt den Frosch nach Links und Rechts laufen. Mit Eat kann der Frosch die Fliege essen. Falling sorgt dafür, dass die Fallgeschwindigkeit immer höher wird. Checkfalling bedeutet, dass überprüft wird, ob der Actor auf einer Platform ist und lässt diesen fallen, wenn dies nicht der Fall ist.

![image](https://user-images.githubusercontent.com/111414678/208299440-5057b6fb-7cf5-48ef-953b-e863b20ce4ba.png)
![image](https://user-images.githubusercontent.com/111414678/208299531-152c0bee-a59e-4d93-ae85-9f57e12dd6d8.png)
![image](https://user-images.githubusercontent.com/111414678/208299539-7aca42f9-a294-440f-8dd2-96db05aa8722.png)



#### GameOver
GameOver ist ein Actor, der ausgeführt wird, wenn der Spieler getötet wird. Er bedeckt dann den Bildschirm mit einem "dead"-Schriftzug in rot-schwarzer Farbe. Dazu erscheint eine akustische Untermalung in Form eines passenden Geräuschs.
![image](https://user-images.githubusercontent.com/111414678/208299554-0970a94d-2e1a-4d37-87f7-f29adfd78b7e.png)


#### Grünkohl
"Grünkohl" ist ein Actor, der vom Spieler gegessen werden kann. Er bewegt sich exakt mit dem Hintergrund durch den move Befehl, der an die Tastaturtasten a und d geheftet wurde.
![image](https://user-images.githubusercontent.com/111414678/208299568-7e2692e4-778f-40be-8270-af50950889ba.png)


#### Infotafel
Auf der Infotafel wird dem Spieler sein Ziel, den Kuchen zu essen mitgeteilt. Sie wurde von uns auf der Seite "pixelart" erstellt und ins Spiel eingefügt. In jedem Level gibt es nahe der Startposition des Spielers eine Infotafel. Sie bewegt sich exakt mit dem Hintergrund durch den move Befehl, der an die Tastaturtasten a und d geheftet wurde.
![image](https://user-images.githubusercontent.com/111414678/208299587-12127aae-48ed-4926-ac6d-5a3043662fd0.png)


#### Kuchen
"Kuchen" ist ein Actor, der vom Spieler gegessen werden kann. Wenn er dies tut, schließt er ein Level ab bzw. gewinnt dieses. Er bewegt sich exakt mit dem Hintergrund durch den move Befehl, der an die Tastaturtasten a und d geheftet wurde.
![image](https://user-images.githubusercontent.com/111414678/208302596-3a7aa52d-fed5-4e26-98ae-07c73dcac56c.png)



#### Minze
"Minze" ist ein Actor, der vom Spieler gegessen werden kann. Er bewegt sich exakt mit dem Hintergrund durch den move Befehl, der an die Tastaturtasten a und d geheftet wurde.
![image](https://user-images.githubusercontent.com/111414678/208299622-46b6cfd8-d089-49e9-b28a-1323c6c448cc.png)



#### Platform
Auf der "Platform" kann der Spieler stehen, sich bewegen und springen ohne nach unten zu fallen.
![image](https://user-images.githubusercontent.com/111414678/208299639-2ec66d0e-f069-466c-a8fa-64fb63dcc9c9.png)



#### Player
Der Actor "Player" ist der vom Spieler gesteuerte Ritter im ersten Level. Wenn dieser Grünkohl oder Minze isst, erscheint ein dazu passendes Geräusch.
![image](https://user-images.githubusercontent.com/111414678/208299750-58f584b4-1cc0-4889-a5b9-0023ecbbc46f.png)
![image](https://user-images.githubusercontent.com/111414678/208299774-e0fc016c-5dd1-458c-93cd-9f95523ceab7.png)
![image](https://user-images.githubusercontent.com/111414678/208299786-12bca19b-e778-4fc3-bebc-8d8104e14221.png)
![image](https://user-images.githubusercontent.com/111414678/208299803-347105f4-9751-4529-9991-14bb1696df53.png)
![image](https://user-images.githubusercontent.com/111414678/208299843-61c2c22e-3966-4b96-94d3-4c367d2d8bc7.png)



#### Player2
Der Actor "Player2" ist der vom Spieler gesteuerte Ritter im zweiten Level.
![image](https://user-images.githubusercontent.com/111414678/208300406-06cf85c6-ef02-4de2-ad14-854704a31952.png)
![image](https://user-images.githubusercontent.com/111414678/208300429-e8006e79-4ae1-46ed-977e-55e1fb457f2f.png)
![image](https://user-images.githubusercontent.com/111414678/208300447-35fa586c-3928-4579-9672-60e069391255.png)
![image](https://user-images.githubusercontent.com/111414678/208300466-fdf23c41-e9e8-4f8d-a8d7-60ad9c4a327e.png)
![image](https://user-images.githubusercontent.com/111414678/208300532-df79d1ba-683b-40f9-a44a-8b13f2261252.png)
![image](https://user-images.githubusercontent.com/111414678/208300554-87115154-befb-43a0-bc87-5a0f0b7c75ef.png)



#### Schlange
Der Actor "Schlange" kann als einziger Actor im ersten Level den Spieler töten. Deshalb ist es für den Spieler nur möglich, ihm auszuweichen, um das Ziel zu erreichen.
![image](https://user-images.githubusercontent.com/111414678/208300606-64226099-4d3f-4b8a-a4ef-2729364a025b.png)
![image](https://user-images.githubusercontent.com/111414678/208300622-43d601c2-d052-437b-8fe1-aa448a9a80b9.png)


#### Schlange2
Dieser Actor ist eine Kopie vom Actor "Schlange". Er ist und macht das gleiche im zweiten Level, wie der Name erkennen lässt.
![image](https://user-images.githubusercontent.com/111414678/208300661-9f1532a8-f361-498d-8a1b-361a5598ace9.png)
![image](https://user-images.githubusercontent.com/111414678/208300674-8f71dc57-35d1-4f23-9040-6b47fb2d82ea.png)


#### Steuerung
Dieser Actor ist eine Infotafel, die sich für den Spielenden nicht bewegt und ihm die Steuerung für den Player zeigt. Sie bewegt sich exakt mit dem Hintergrund durch den move Befehl, der an die Tastaturtasten a und d geheftet wurde.
![image](https://user-images.githubusercontent.com/111414678/208300764-e4d98552-d08f-4626-8be0-2e3288628b82.png)


#### WinOver
"WinOver" ist ein Actor, der ausgeführt wird, wenn der Actor Kuchen getötet wird bzw., wenn der Spieler den Kuchen isst. Er bedeckt dann den Bildschirm mit einem "win"-Schriftzug in grün-schwarzer Farbe. 
![image](https://user-images.githubusercontent.com/111414678/208300782-d710ba65-fd03-44f4-b5f6-d275fb5a87a3.png)

