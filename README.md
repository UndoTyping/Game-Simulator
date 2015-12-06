# Game-Simulator
 C#


World {
	protected Game_Object[] world;
	ShowWorld() virtual;
}

World2d based on World {
	
}

// King, Queen, Plan
Game_Object {
	Coordinates coordinates;
	Player player;
	Set(Coordinates)
}

Plane based on Game_Obejct {
	azimute
	alt
	Coordinates
	NextMove()
}

Game {
	Game_Obejct[] Game_Objects;
	Init(); // i.e. Place Chess object in the world
	Start() {
	Player[] Plays;
	foreach player {
		Game.Next_Move();
		Player[i].Next_Move();
		ShowWorld();
		Check_Win();
	}
	}
	NextMove() {
		foreach Game_Object [
			Game_Object.NextMove()
		]
	}
	Player CheckWin() virtual;
}

XmixZrix based Game {

}

Chess based Game {
	Set 
	Check_Gold(Coordinate)

}

class Player {
	Coordinates (x,y)
	Inventory 
	Next_Move() virtual
}

class PlayerA based on Player {
	Next_Move() {
		if (x<5)
			Check_Gold()
}
}

Main {
}
	
