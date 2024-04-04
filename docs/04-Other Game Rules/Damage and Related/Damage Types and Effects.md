# Damage Types and Effects
________________________________________
________________________________________

## Base Info

Specifications:
-	Normal effect: non-crit effect
-	Special effect: usually applied on crit or SE roll success
-	AMR Block:  Damage nullification by armor
-	Resistance Chance (Damage): damage weakness/resistance
-	Resistance Chance (Condition): Effect weakness/resistance

Damage Type Amounts:
-	Physical (5)
-	Elemental (10)
-	Resource-Based (6)
-	Unique (3)

## Damage Types
### **Physical

#### [[Bludgeon]]
-	Special effect: Clumsy
	-	50% chance to drop item you are holding or using
	-	50% chance to apply Condition: Prone (Lingering) during Movement Actions
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Lacerate]]
-	Special effect: Bleed (DOT)
	-	Victim bleeds their HP
	-	Bleed \[2] HP per physical action and for each unit moved (Push does not count)
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Lash]]
-	Special effect: Disable
	-	Unable to use Weapons and Items
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Pierce]]
-	Normal effect: Basic
-	Special effect: Cleave 
	-	\[20]% of IncomingDamage will always ignore defenses (round down)
	-	Note:
		-	==This does NOT add damage==
		-	Even if all damage is blocked, X damage will still be received
-	AMR Block: False
-	Resistance Chance (Damage): False
-	Resistance Chance (Condition): False
 
#### [[Slash]]
-	Special effect: Offwind: 
	-	When target is damaged, entities within 1-by-3 units on opposite side of attack take half IncomingDamage value
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): False

---
### **Elemental

#### [[Cold]]
-	Special effect: Chill
	-	NIM and Speeds cut by 50%.
	-	Cancelled out with Heated
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Corrosive]]
-	Special effect: Frail
	-	CON and \[all Block/Resistances] cut by 50%
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Force]]
-	Special effect: Push
	-	Knockback: moves X units back
	-	X=1 unit by default if not specified
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Heat]]
-	Special effect: Flame (DOT)
	-	Each application of Flame adds 4 stacks
	-	Applied stacks = Damage
	-	At end of each round flame damage is applied
	-	1 stack removed each round 
		-	if stack = 0, Flame ends
	-	Condition: Drenched (Water) and \[stop, drop, and roll] removes Flame
		-	\[stop, drop, and roll]:  
			-	1AP/RP = roll 1d6
				-	1 = remove no Flame stacks, use 1 additional AP/RP
				-	2 = remove no Flame stacks
				-	3 = remove half Flame stacks
				-	4 = remove half Flame stacks
				-	5 = remove All Flame stacks
				-	6 = remove All Flame stacks, refund 1 AP/RP
	-	If Flamed target has Condition: Drenched (Oil) 
		-	 \[stop, drop, and roll]  will not work.
		-	Application adds 8 Flame stacks
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Necrotic]]
-	Special effect: Wither
	-	Apply \[up to 20] Jam(medHP) per Application
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Radiant]]
-	Special effect: Burn
	-	Bonus damage of \[4] added to DamageInstances.
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Shock]]
-	Special effect: Disorient: 
	-	PER cut by 50%, 
	-	Stealth roll disadvantage
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Sound]]
-	Special effect: Vertigo
	-	RE: \[-25] ACC
	-	RE: \[-25] Dodge
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Toxic]]
-	Special effect: Poisoned (DOT) 
	-	Poison # (60 max) is damage at the end of your turn
		-	Damage is blocked by BSI: \[Poison-BSI] =\[Damage]
			-	Will take still take 1 DOT even if BSI blocks all damage
	-	If you are hit with multiple applications of poison: 
		-	You take the highest raw Poison value (even if you already have poison)
		-	Poison Applications do not stack
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Umbral]]
-	Special effect: Weakness
	-	STR and PWR reduced by 50%
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

---
### **Resource-Based

#### [[Anti-Myrr]]  
-	Special effect: MyrrCrash 
	-	When entity uses Myrr, entity takes damage based on Myrr amount
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Blight]]
-	Special effect: Rabid
	-	Cannot use communication
	-	fail social abilities
	-	Fail impulse checks 
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Aeonic]]
-	Special effect: Infernum
	-	Application applies 4 stacks
	-	Applied stacks = Damage
	-	At end of your turn, stack damage is applied
		-	+1 stack added at the start of your turn
	-	To remove:
		-	roll 1d10 (cost 1 AP/RP)
		-	roll equal to stacks removed
		-	When stack = 0, Infernum is removed
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): False

#### [[Mental]]
-	Special effect: Confusion
	-	Gain 5 Stress
	-	When using abilities, after rolling for ACC (Hit or Miss) and PWR, coinflip to see if you target yourself
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Myrr]]
-	Special effect: MyrrSap 
	-	Absorb 1d10 Myrr from non-drained environment
	-	Doesn’t work in an Anti-Myrr field
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True

#### [[Spectral]]
-	Special effect: Missfire
	-	All (targeted) abilities have a chance to miss
	-	When using abilities: 
		-	Roll for resource use
		-	Then roll to see if you hit or miss 
			-	If you miss, resource is still used
-	AMR Block: True
-	Resistance Chance (Damage): True
-	Resistance Chance (Condition): True
 
---
### **Unique

#### [[Splash]]
-	Normal effect: 
	-	damage always AOE (at least 1 unit radius, if damage/attack/ability isn’t already AOE)
	-	radius deals 20% of damage instance (if damage/attack/ability isn’t already AOE)
		-	AMR Block: True
		-	Resistance Chance (Damage): True
		-	Resistance Chance (Condition): False
-	Special effect: Blast
	-	AOE Range: Doubled
	-	AOE Damage:  10% of damage instance
	-	==Blast Effect: All other Special Effects that activate for initial target during attack happens/applies to all in AOE==
		-	AMR Block: True
		-	Resistance Chance (Damage): True
		-	Resistance Chance (Condition): False

#### [[Vampiric]]
-	Normal effect: 
	-	each instance of (melee) damage dealt heals you for 1 HP
		-	AMR Block: False
		-	Resistance Chance (Damage): False
		-	Resistance Chance (Condition): False
-	Special effect: Lifesteal 
	-	Heal 1d10 \[auto2] if (melee) damage is dealt
	-	Note: Specifics can vary
		-	AMR Block: False
		-	Resistance Chance (Condition): False

#### [[True]] 
-	Normal effect: always Ignores/overrides all defenses and resistances
-	Special effect: N/A
-	AMR Block: False
-	Resistance Chance (Damage): False
-	Resistance Chance (Condition): False
