# Related Damage Info
________________________________________
________________________________________

## Guide:
-	Armor = AMR	
-	IncomingDamageInstance = IDI
-	CombinedDamageInstance = CDI
-	ReceivedDamage = RD
-	Minimum = Min

## Block and Damage Instances
### Block
Block negates each instance of incoming damage, not the sum of damage.
For a single instance:
-	\[IDI]-\[Block] = \[RD (1min)]

### Multiple Instances
For multiple instances (MultiHit), \[RD (min = 1 per Damage Instance)]
-	For example, 2 instances: \[(IDI)-(Block)] + \[(IDI)-(Block)] = \[RD (min = 2 )]

If multiple instances of damage hit at once they can count as one instance (ComboDamage).
-	\[(CDI)+( CDI)]-\[Block] = \[Sum of CDIs]-\[Block] = \[RD(1min)]

### Shield Buffer
-	Even if you block all incoming damage, you will take 1 point of damage. 
-	This is to ensure there are no “brick wall” scenarios, where people fight but no damage is applied because their block is high enough. 
-	Only certain abilities counter this.

### Miscellaneous
-	Damage Over Time (DOT) effects ignore Block after initial damage is applied. 
-	All Incoming Damage is negated by Block except for True Damage.

## Mixed Types and Combined Damage

### Mixed Types
When multiple damage and resistance types ae calculated together for the same amount note that: 15XY is different from 10X+5Y
### Damage Resistances 
There are several types of damage that can be implemented. Paying attention to damage type weaknesses, resistances, immunities and  and typing combinations will be important. If an attack has multiple damage types, all resistances and weaknesses towards that type are calculated and summed along with Block. If your character is immune to damage type, they still take 1 damage from said type due to shield buffer. 
-	10 Incoming\[Type1+Type2]Damage - \[4(Type1)Resist+3(Type2)Resist] = 3RD
-	10 Incoming\[Type1+Type2]Damage – 7TotalResist = 3RD

## Noted Info:

### Quick Fractional Calculations
10%: 
-   Calculate number, then divide by 10 (round down)
	-   Alternatively, calculate number then move decimal left by one space (tens)
-   ex.  10% of 100: 100 / 10 = 10

20%:
-   Follow steps for 10% calculation, then multiply rounded # by 2

50%:
-   Calculate number, then divide by 2 (round down)

### [[Absolute Value]]
The distance between a number and the origin (zero) on a number line; it is always non-negative. 
A number (#), variable (X, Y, Etc.), or term between 2 vertical bars indicates an Absolute Value

### Multihit Calculations
-	Main Multihit operation (True-Streamlined)
	-	Roll if hit was successful (Hit/Miss)
	-	Roll to determine the # of attacks that hit the target(s). (roll 1d\[the lowest possible die] for what is needed) (Accuracy)
	-	Roll for Damage; # applies to all connecting hits (that hit the target)
	-	Roll Special Effect; apply to all connecting hits (that hit the target)
	-	Do bonus (damage) rolls after initial damage rolls. Can split bonus damage between instances.
-	Semi Individual operation (Semi-Streamlined)
	-	Roll if hit (Hit/Miss)
	-	Roll for # of attacks that hit.(roll 1d\[the lowest possible die] for what is needed) (Accuracy)
	-	Roll for Damage and Special Effect for each connecting hit
	-	Do bonus (damage) rolls after initial damage rolls. Can split bonus damage between instances.

