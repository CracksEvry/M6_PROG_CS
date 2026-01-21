# Progopdrachten M6

## Opdracht 1 / Code Conventions

[Script/Code](https://github.com/CracksEvry/M6_PROG_CS/tree/main/Assets/Scripts/M6/Code%20Conventions)


## Opdracht  2 / Class diagram Towerdefense

```mermaid

classDiagram

class Bullet {
    - int damage
    - float lifeTime
    + Start()
    + OnTriggerEnter2D(collider)
}

class Enemy {
    - int health
    - int cashReward
    - spriteRenderers
    - Transform visuals
    + TakeDamage(dmg)
    + KillEnemy()
    + FlashEffect()
}

Bullet --> Enemy : interacts with


	

	

```


## Opdracht 3 / Data Structures

[Script/Code](https://github.com/CracksEvry/M6_PROG_CS/tree/main/Assets/Scripts/M6/Data%20Structure)

## Opdracht 4 / delegates gebruiken

![ezgif-75d548983100605b](https://github.com/user-attachments/assets/94446952-1f43-45df-9127-c695027c6842)


[Delgates](https://github.com/CracksEvry/M6_PROG_CS/tree/main/Assets/Scripts/M6/Delegates)

```Charp
public bool IsPlayerReadyToAttack(Player player)
{

        if (player == null) return false;
        if (!player.IsAlive) return false;
        if (player.AttackCooldown > 0) return false; 
        if (player.Target == null) return false;

        if (!player.Target.IsAlive) return false;

   
    if (Vector3.Distance(player.transform.position, player.Target.transform.position) >= 5f)
    {
        return false;
    }

    bool hasManaAndWeapon
        if (player.Mana >= 20 && player.HasEquippedWeapon("Sword"))
    hasManaAndWeapon = true;
    
    bool hasHealthAndBuff
        if (player.Health >= 50 && player.HasActiveBuff("RageMode"))
        hasHealthAndBuff = true;

        if (!hasManaAndWeapon || !hasHealthAndBuff)
        
     return true;
    



}
```

## Opdracht 5 / Abstractions


![asnd](https://github.com/user-attachments/assets/b15cf525-8f94-425c-a398-9a9443007e75)



[Script/Code](https://github.com/CracksEvry/M6_PROG_CS/tree/main/Assets/Scripts/M6/Abstraction)



## Opdracht 6 / Polymorfisme

![asdna](https://github.com/CracksEvry/M6_PROG_CS/blob/main/GIFS%20ETC/Opdracht6%20Pholomon.gif)



[Script/Code](https://github.com/CracksEvry/M6_PROG_CS/tree/main/Assets/Scripts/M6/Polymorfisme)


## Opdracht 7 / Early Returns

![kajsndkansd]