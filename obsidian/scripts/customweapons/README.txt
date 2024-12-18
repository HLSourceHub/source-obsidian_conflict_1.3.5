Scripted Weapons.
All names should start with custom_ for them to be loaded correctly. If you dont, the weapon will use its default properties.
Also, all custom weapon scripts should be placed in this folder.

Only the weapon_scripted entity can use the "Advanced" configurations. All others will only use the basic configurations.

// LIST OF USABLE ADVANCED SECTION VALUES \\

// **Primary Attack**

// 0 = none, 1 = Basic Bullet, 2 = Burst, 3 = shotgun, 9 = NadeType
"FireType1"	"1"


// Rate of Weapons Fire ( Not for laser or warp )
"FireRate1"	"0.1"

// Allow a refire as fast as the player can click, Basic Bullet Only.
"FastFire1"	"0"

// Allow Fire Underwater?
"FireUnderWater1"	"0"

// How many bullets in a burst. ( For Burst Weapon Only! )
"BurstAmount1"	"0"
"BetweenBurstTime1"	"0.05"

// For Bullet accuracy
"FireCone1"		"2" // Starting Value ( 0-20 )
"FireConeLerp1"		"1" // Bool, should be 1 to use lerp
"FireConeLerpto1"	"6" // Value to lerp accuracy too ( 0-20 )

// **Secondary Attack**

// 0 = none, 1 = Basic Bullet, 2 = Burst, 7 = scope, 8 = Launch Nade
"FireType2"	"2"

// Rate of Weapons Fire ( Not for laser or warp )
"FireRate2"	"0.7"

// Allow a refire as fast as the player can click, Basic Bullet Only.
"FastFire2"	"0"

// Allow Fire Underwater?
"FireUnderWater2"	"0"

// How many bullets in a burst. ( For Burst Weapon Only! )
"BurstAmount2"	"4"
"BetweenBurstTime2"	"0.05"

// Secondary Fire uses Secondary Ammo Type. If 0, will use primary ammo.
"SecondaryAmmoUsed"	"0" //( NOT YET FUNCTIONAL )

// For Bullet accuracy
"FireCone2"		"2" // Starting Value ( 0-20 )
"FireConeLerp2"		"1" // Bool, should be 1 to use lerp
"FireConeLerpto2"	"6" // Value to lerp accuracy too ( 0-20 )

// **Global Weapon Settings**

// Number of Recoil Animations, weapon models with ACT_VM_RECOIL animations.
// ( Only if a weapon has recoil animations, Not for laser or warp )
"NumberOfRecoilAnims"	"0"

// Shots fired till next recoil animation. ( Only if a weapon has recoil animations )
"RecoilIncrementSpeed"	"1"

// 1 = Pistol, 2 = AR2, 3 = crossbow, 4 = physgun, 5 = shotgun, 6 = smg1, 7 = nade
// This is the player animation set that will be used on all players you view ingame.
"PlayerAnimationSet"	"2"

// Grenade Damage
"GrenadeDamage"	"100.0"

// Grenade Radius
"GrenadeRadius"	"250.0"

//Tracer type ( Bullet weapons only )
// 0 = none, 1 = normal, 2 = strider, 3 = ar2, 4 = helicopter, 5 = Gunship, 6 = Gauss, 7 = Airboat
"TracerType"	"1"

//Tracer Frequency
"TracerFrequency"	"2"

// Bullet Impact Effect, 0 = none, 1 = normal, 2 = AR2, 3 = jeep, 4 = Gauss, 5 = airboat, 6 = helicopter
"ImpactEffect"	"1"

// Sniper Scope Settings
"UseScopedFireCone"	"1"
"ScopedFireCone"	"0"
"ScopedColorR"		"255"
"ScopedColorG"		"255"
"ScopedColorB"		"255"

// **NPC Weapon Settings**

// NPCs use a ShotRegulator in code, these settings corrispond with it.
"NPCRateofFire"		"0.1"
"NPCMinBursts"		"1"
"NPCMaxBursts"		"3"
"NPCMinRest"		"0.3"
"NPCMaxRest"		"0.6"

// Range the NPC can fire this weapon at, if the player is less than min, the npc cant fire and will try to get a better vantage point.
"NPCMinRange1"		"24"
"NPCMaxRange1"		"1500"
"NPCMinRange2"		"24"
"NPCMaxRange2"		"200"

// **Nadetype ( "FireType1"	"9" options )**

// 1 = frag
"HandNadetype"		"1"

"HandNadeTimer"		"2.5"
"HandNadeRadius"	"4.0" // This corresponds with the radius of the nade model, not the damage.
"HandNadeDmgRadius"	"250.0"
"HandNadeDmg"		"150.0"
