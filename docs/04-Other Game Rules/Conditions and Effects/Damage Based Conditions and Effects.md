# Damage Based Conditions and Effects
________________________________________
________________________________________

### **Damage Based Conditions**
#### [[Bleed]]
-	Resistance Chance (Condition): True
-	Victim bleeds their HP
-	Bleed \[2] HP per physical action and for each unit moved (Push does not count)

#### [[Burn]]
-	Resistance Chance (Condition): True
-	Bonus damage of \[4] added to DamageInstances.

#### [[Chill]]
-	Resistance Chance (Condition): True
-	NIM and Speeds cut by 50%.
-	Cancelled out with Condition: Heated

#### [[Clumsy]]
-	Resistance Chance (Condition): True
-	50% chance to drop item you are holding or using
-	50% chance to apply Condition: Prone (Lingering) during Movement Actions

#### [[Confusion]]
-	Resistance Chance (Condition): True
-	Gain 5 Stress
-	When using abilities, after rolling for ACC (Hit or Miss) and PWR, coinflip to see if you target yourself

#### [[Disable]]
-	Resistance Chance (Condition): True
-	Unable to use Weapons and Items

#### [[Disorient]]
-	Resistance Chance (Condition): True
-	PER cut by 50%
-	Stealth roll disadvantage

#### [[Flame]]
-	Resistance Chance (Condition): True
-	Each application of Flame adds 4 stacks
-	Applied stacks = Damage
-	At start of each round flame damage is applied
-	1 stack removed each round 
	-	if stack = 0, Flame ends
-	Condition: Drenched(Water) and \[Stop, Drop, and Roll] removes Flame
	-	Stop, Drop, and Roll:  
		-	1AP/RP = roll 1d6
			-	1 = remove no Flame stacks, use 1 additional AP/RP
			-	2 = remove no Flame stacks
			-	3 = remove half Flame stacks
			-	4 = remove half Flame stacks
			-	5 = remove All Flame stacks
			-	6 = remove All Flame stacks, refund 1 AP/RP
-	If Flamed target has Condition: Drenched(Oil)
	-	 \[Stop, Drop, and Roll] will not work.
	-	Application adds 8 Flame stacks

#### [[Frail]]
-	Resistance Chance (Condition): True
-	CON and \[all Block/Resistances] cut by 50%

#### [[Infernum]]
-	Resistance Chance (Condition): False
-	Application applies 4 stacks
-	Applied stacks = Damage
-	At end of your turn, stack damage is applied
	-	+1 stack added at the start of your turn
-	To remove:
	-	roll 1d10 (cost 1 AP/RP)
	-	roll equal to stacks removed
	-	When stack = 0; Infernum is removed

#### [[Missfire]]
-	Resistance Chance (Condition): True
-	All (targeted) abilities have a chance to miss
-	When using abilities: 
	-	Roll for resource use
	-	Then roll to see if you hit or miss 
		-	If you miss, resource is still used

#### [[MyrrCrash]] 
-	Resistance Chance (Condition): True
-	When entity uses Myrr, entity takes damage based on Myrr amount

#### [[MyrrSap]]
-	Resistance Chance (Condition): True
-	Absorb 1d10 Myrr from non-drained environment
-	Doesn’t work in an Anti-Myrr field

#### [[Poisoned]]
-	Resistance Chance (Condition): True
-	Poison # (60 max) is damage at the end of your turn
	-	Damage is blocked by BSI: \[Poison-BSI] = \[Damage]
		-	Will take still take 1 DOT even if BSI blocks all damage
-	If you are hit with multiple applications of poison: 
	-	You take the highest raw Poison value (even if you already have poison)
	-	Poison Applications do not stack

#### [[Push]]
-	Resistance Chance (Condition): True
-	Knockback: moves X units back
-	X=1 unit by default if not specified

#### [[Rabid]]
-	Resistance Chance (Condition): True
-	Cannot use communication
-	Fail social abilities
-	Fail impulse checks 

#### [[Vertigo]]
-	Resistance Chance (Condition): True
-	RE: \[-25] ACC
-	RE: \[-25] Dodge

#### [[Weakness]]
-	Resistance Chance (Condition): True
-	STR and PWR reduced by 50%

#### [[Wither]]
-	Resistance Chance (Condition): True
-	Basics
	-	Apply \[up to 20] Jam(medHP) per Application
-	HP
	-	\# = new health limit
	-	If current HP goes under Jam-Wither, you enter limbo
		-	If you current HP goes above Wither #, you exit the wither-induced limbo
		-	If wither # decreases, you MAY exit wither-induced limbo

### **Damage Based Effects**

#### [[Blast]]
-	Resistance Chance (Condition): False
-	AOE Range: Doubled
-	AOE Damage:  10% of damage instance
-	==Blast Effect: All other Special Effects that activate for initial target during attack happens/applies to all in AOE==
#### [[Cleave]]
-	Resistance Chance (Condition): False
-	\[20]% of IncomingDamage will always ignore defenses (round down)
-	Note:
	-	==This does NOT add damage==
	-	Even if all damage is blocked, X damage will still be received

#### [[Lifesteal]]
-	Resistance Chance (Condition): False
-	Heal 1d10 \[auto2] if (melee) damage is dealt
-	Note: Specifics can vary

#### [[Offwind]]
-	Resistance Chance (Condition): False
-	When target is damaged, entities within 1-by-3 units on opposite side of attack take half IncomingDamage value

#### [[Perforate]]
-	Resistance Chance (Condition): False
-	AOE
-	Attack goes through all entities along path, applying damage (and effects)

#### [[Splash]]
-	Resistance Chance (Condition): False
-	Damage always AOE (at least 1 unit radius, if damage/attack/ability isn’t already AOE)
-	Radius deals 20% of damage instance (if damage/attack/ability isn’t already AOE)


