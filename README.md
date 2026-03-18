void ComparePlayer(List<GameObject> players)
{
   //+1 init, +(N+1) Comparaciones, +N incrementos = 2N + 2
	
   for (int i = 0; i < players.Count; i++)
{

   for (int j = i + 1; j < players.Count; j++)
{ 
    Debug.log(players[i].name + " vs " + __________);
      }
   }
}
SOLUCION:
FOR INTERNO: 4N +6
(4N + 6)N
4N al cuadrado + 6 + 1 + N+1 + N
TO = 4N² + 8
ON = N²



Ejercicio 2:

int calculateInteractionScore (int [] players)
{
  int score= 0
  for (int i = 0; i < players.length; i++)
  {
    for (int j = i + 1; j < players.length; j++)
    {
       int  interaction = players[i] + players[j];
       score += interaction;
       }
  }

SOlUCION:
1+N+1+N+1+N+1+N
N(6+4N)
4N²+ 6N

1+1+N+1+N+4N²+6N+1 = 4N² + 8N + 4

EJERCICIO 3:
int CalculateFinalDamage( int Attack, int defense, float multipliear)
{
int BaseDamage = attack - defense;
int finalDamage = (int)(baseDamage * multiplier);

if (finalDamage < 0)
{
finalDamage = 0;
}
return finalDamage;
}

















