# FuryTech
________________________________________
________________________________________

## Main Info

Fury is a unique Energy in that it is only gained in combat. While most Fury abilities are only used in combat, some can be use outside of combat.

In (Physical) Combat:
-	Fury Users automatically gain (10\[lv 1-5], 20\[lv 6-10], 30\[lv 11-15], 40\[lv 16-20], 50\[lv 21-25], 60\[lv 26-30]) fury at the start of battle.
-	Fury is gained from:
	-	10% of all damage taken 
	-	10% of melee damage dealt 
-	You cannot gain Fury from:
	-	abilities using Fury as a resource
	-	abilities enhanced by Fury
-	When under 5% HP, become Immune to DOTs

Outside of Combat
-	After combat ends, user can store up to (10\[lvl1-3], 20\[lvl4-6], 30\[lvl7-9], 40\[lvl10-12], 50\[lvl13-15], 60\[lvl16-18] 70\[lvl19-21] 80\[lvl22-24] 90\[lvl25-27] 100\[lvl28-30]) of their remaining Fury.
-	Rests remove all remaining Fury.

Note: Furian classes may have enhanced/additional abilities if Fury is the users main Energy

## **Abilities**

### Fury Abilities: Usable Out-of-Combat

#### Blood Boil
-	Trait: Active
-	Action Cost: 1AP
-	Range: self
-	Components: 
-	Impact: Tangible
-	Duration:  Instant
-	Use: Regular
-	Resource: Fury: up to (20\[lv 1-6], 40\[lv 7-12], 60\[lv 13-18], 80\[lv 19-24], 100\[lv 25-30])
-	Prerequisite: Energy: Fury
-	Description: 
	-	Clear \[Resource/2] wither
	-	Clear \[Resource/2] poison  
	-	-5 HP
	-	Note: round down on odd number results	

#### Burning Passion
-	Trait: Active
-	Action Cost: Free
-	Range: self
-	Components: 
-	Impact: Tangible
-	Duration:  Concentration (>50)
-	Use: Regular
-	Resource: Fury: (1\[1-5], 3\[6-10], 5\[11-15], 10\[16-20], 20\[21-25], 25\[26-30]) per round
-	Prerequisite: Energy: Fury
-	Description:  
	-	Ignore DOT effects
		-	Effects are suspended within your body
		-	You do not take damage from these effects
	-	If Concentration fails, you must wait until the next turn to try again

#### BattleFury
-	Trait: Active
-	Action Cost: 0.5 AP
-	Range: self
-	Components: 
-	Impact: Tangible
-	Duration:  Instant
-	Use: Regular
-	Resource:  X Fury
-	Prerequisite: Energy: Fury
-	Description: 
	-	Use fury to heal yourself or increase melee damage 
		-	Heal \[Resource] Amount
			-	If you go over Safe Limit, the next round you 
				-	take 25% of heal amount as bonus damage per IncomingDamage instance
				-	gain no fury
		-	Increase next melee damage (PWR) by \[Resource] 
			-	If you go over Safe Limit, you will take 25% damage you deliver. 
				-	This does not give you Fury
			-	If you miss, empowerment is still used up
	-	Note: Have a Safe Limit of (5\[lv 1-5], 10\[lv 6-10], 15\[lv 11-15], 20\[lv 16-20], 25\[lv 21-25], 30\[lv 26-30])

### Fury Abilities: Combat Only

#### Blood Cry
-	Trait: Active
-	Action Cost: 1AP
-	Range: self, 5 unit(s)
-	Components: vocal, in combat
-	Impact: Intangible
-	Duration:  Instant
-	Use: 5 uses per Combat
-	Resource: 50
-	Prerequisite: Energy: Fury
-	Description: 
	-	Applies Vertigo to nearby enemies
	-	-20 Stress to self	

#### Tranquil Fury
-	Trait: Active
-	Action Cost: 1AP
-	Range: self
-	Components: in combat
-	Impact: Intangible
-	Duration:  Instant
-	Use: 5 uses per Combat
-	Resource: 100
-	Prerequisite: Energy: Fury
-	Description: 
	-	gain enforced Zen:SoM or Anger:SoM
	-	your choice of SoM, no roll

#### Fighting Focus
-	Trait: Active
-	Action Cost: Free
-	Range: self
-	Components: in combat
-	Impact: Mix
-	Duration:  1 Round
-	Use: 5 uses per Combat
-	Resource: Fury: 100
-	Prerequisite: Energy: Fury
-	Description: 
	-	Empower your next Melee attack 
		-	IncomingDamage x2
		-	RE: +25 ACC
	-	If you miss, empowerment is still used up	

#### Furious Spirit
-	Trait: Active
-	Action Cost: Free
-	Range: self
-	Components: in combat
-	Impact: Mix
-	Duration:  Instant
-	Use: 5 uses per Combat
-	Resource: Fury: 100
-	Prerequisite: Energy: Fury
-	Description: 
	-	Clear all Incapacitations and target altering Conditions 
	-	Consumes all Fury

#### Battle Purification
-	Trait: Active
-	Action Cost: 2AP
-	Range: self
-	Components: in combat
-	Impact: Mix
-	Duration:  Instant
-	Use: 1 uses per Combat
-	Resource: Fury: 200
-	Prerequisite: Energy: Fury
-	Description: 
	-	Clears Emotion
	-	Removes All Conditions
	-	Consumes all Fury	

#### Frustration Dance
-	Trait: Active
-	Action Cost: Free
-	Range: self
-	Components: in combat
-	Impact: Mix
-	Duration:  Toggle
-	Use: Regular
-	Resource: Fury: Free
-	Prerequisite: Energy: Fury
-	Description: 
	-	While active:
		-	When an attack misses, player gains a stack.
			-	1 stack equates to \[3 (under lvl15), 5(lvl15 and up)] Stress and potential bonus damage.
			-	Stacks are automatically applied to Stress
		-	When an attack hits, all Stacks are consumed. 
			-	Stacks applied as Bonus damage to attack (if multihit applies to all instances after confirmed hit)
			-	X Stress removed
		-	Attacks must be melee and tangible.

