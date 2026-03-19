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

SOLUCION:

2+2+1+1+1
7

T(N) = 7
O(N) = 1

EJERCICIO 4:
int SumScores(int[] scores)
{
    // +1 (asignación)
    int sum = 0;
    //+1 init, +(N+1) comparaciones, +N incrementos = 2N + 2
    for (int i = 0; i < scores.Length; i++)
    {
        //+2 (acceso + suma) + N = N+2
        sum += scores[i];
    }
    


1+(2N+2)+(N+2)+1
3N+6

T(N) = 3N+6
O(N) = N



Ejercicio 5:

int CountStrongerPairs(int[] powerLevels)
{
    //+1 (asignación)
    int count = 0;

    //+1 init, +(N+1) comparaciones, +N incrementos = 2N + 2
    for(int i = 0; i < powersLevels.Length; i++)
    {
        //+1 init, +(N+1) comparaciones, +N incrementos = 2N + 2
        for(int j = 0; j < powersLevels.Length; j++)
        {
            //+N, +1 (comparación), +N = 2N +1
            if(powerLevels[i] > powerLevels[j])
            {
                //+N
                count++;
            }
        }
    }
    //+1 (llamada simple)
    return count;
}

Interno:
2N+2+(2N+1)+N
N(5N+3)
5N²+3N

Externo:
1+2N+2(5N²+3N)+1
5N²+5N+4

T(N) = 5N²+5N+4
O(N) = N²

EJERCICIO 6:

bool HasLowHealthPlayer(int[] healthValues)
{
    //+1 init, +(N+1) comparaciones, +N incrementos = 2N + 2
    for(int i = 0; i < healthValues.Length; i++)
    {

        //+1 (acceso), +N = N + 1
        int health = healthValues[i];

        //+1 (comparación)
        if(health < 30)
        {
            //+1 (llamada simple)
            Debug.Log("Low health detected");
            //+1 (llamda simple)
            return true;
        }

    }
    //+1 (llamada simple)
    return false;
}

2N+2+(N+1)+1+1+1+1
3N+7

T(N) = 3N+7
O(N) = N

EJERCICIO 7:

bool CanCastSpeel(int mana, int cost)
{
    //+1 (acceso), +1 (resta) = +2
    int remainingMana = mana - cost;

    //+1 (comparación)
    if (remaingMana >= 0)
    {
        //+1 (llamado simple)
        Debug.Log("Spell casted");
        //+1 (llamado simple)
        return true;
    }

    //+1 (llamada simple)
    return false;

}
2+1+1+1+1
6

T(N) = 6
O(N) = 1


















