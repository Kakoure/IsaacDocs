---
tags:
  - Class
---
# Class "EntityProjectile"

???+ info
    You can get this class by using the following function:

    * [Entity.ToProjectile()](Entity.md#toprojectile)
    * [EntityNPC.FireBossProjectiles()](EntityNPC.md#firebossprojectiles)

    ???+ example "Example Code"
        `local entity = Isaac.GetRoomEntities()[1]:ToProjectile()`

## Class Diagram
--8<-- "docs/snippets/EntityClassDiagram.md"
## Functions
### Add·Change·Flags () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddChangeFlags ( [ProjectileFlags](enums/ProjectileFlags.md) Flags ) {: .copyable aria-label='Functions' }

See [ChangeFlags](#changeflags).
___
### Add·Falling·Accel () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddFallingAccel ( float Value ) {: .copyable aria-label='Functions' }

___
### Add·Falling·Speed () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddFallingSpeed ( float Value ) {: .copyable aria-label='Functions' }

___
### Add·Height () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddHeight ( float Value ) {: .copyable aria-label='Functions' }

___
### Add·Projectile·Flags () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddProjectileFlags ( [ProjectileFlags](enums/ProjectileFlags.md) Flags ) {: .copyable aria-label='Functions' }

You can change the attributes of the projectile by adding one or more [`ProjectileFlag`](enums/ProjectileFlags.md).

___
### Add·Scale () {: aria-label='Functions' }
[ ](#){: .alldlc .tooltip .badge }
#### void AddScale ( float Value ) {: .copyable aria-label='Functions' }

___
### Clear·Projectile·Flags () {: aria-label='Functions' }
[ ](#){: .reporplus .tooltip .badge }
#### void ClearProjectileFlags ( [ProjectileFlags](enums/ProjectileFlags.md) Flags ) {: .copyable aria-label='Functions' }

___
### Has·Projectile·Flags () {: aria-label='Functions' }
[ ](#){: .reporplus .tooltip .badge }
#### boolean HasProjectileFlags ( [ProjectileFlags](enums/ProjectileFlags.md) Flags ) {: .copyable aria-label='Functions' }

___
## Variables
### Acceleration {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float Acceleration  {: .copyable aria-label='Variables' }

___
### Change·Flags {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### [ProjectileFlags](enums/ProjectileFlags.md) ChangeFlags  {: .copyable aria-label='Variables' }

Uses [ProjectileFlags](enums/ProjectileFlags.md) to define the projectile attributes after the "Changed" state was activated.
The [ProjectileFlag](enums/ProjectileFlags.md).CHANGE_FLAGS_AFTER_TIMEOUT needs to be set to allow for this change to apply!
____
**Informations about "Changed" State:**

Projectiles can have two states: normal (default) and changed.


Changed state activates when projectile's frame count reaches the value set in [ChangeTimeout](#changetimeout). After that its flags get changed to what was set in [ChangeFlags](#changeflags) and velocity will be resized to length set in [ChangeVelocity](#changevelocity).
____
Also used in: [ProjectileParams()](ProjectileParams.md)
___
### Change·Timeout {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### int ChangeTimeout  {: .copyable aria-label='Variables' }

Number of frames that need to elapse after spawn till the "Changed" state is activated.
The [ProjectileFlags](enums/ProjectileFlags.md).CHANGE_FLAGS_AFTER_TIMEOUT or CHANGE_VELOCITY_AFTER_TIMEOUT need to be set to allow for this change to apply!
____
**Informations about "Changed" State:**

Projectiles can have two states: normal (default) and changed.


Changed state activates when projectile's frame count reaches the value set in [ChangeTimeout](#changetimeout). After that its flags get changed to what was set in [ChangeFlags](#changeflags) and velocity will be resized to length set in [ChangeVelocity](#changevelocity).
____
Also used in: [ProjectileParams()](ProjectileParams.md)
___
### Change·Velocity {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float ChangeVelocity  {: .copyable aria-label='Variables' }

Velocity value that gets applied when the "Changed" state is activated.
The [ProjectileFlag](enums/ProjectileFlags.md).CHANGE_VELOCITY_AFTER_TIMEOUT need to be set to allow for this change to apply!
____
**Informations about "Changed" State:**

Projectiles can have two states: normal (default) and changed.


Changed state activates when projectile's frame count reaches the value set in [ChangeTimeout](#changetimeout). After that its flags get changed to what was set in [ChangeFlags](#changeflags) and velocity will be resized to length set in [ChangeVelocity](#changevelocity).
____
Also used in: [ProjectileParams()](ProjectileParams.md)
___
### Curving·Strength {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float CurvingStrength  {: .copyable aria-label='Variables' }

___
### Damage {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float Damage  {: .copyable aria-label='Variables' }

___
### Depth·Offset {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float DepthOffset  {: .copyable aria-label='Variables' }

___
### Falling·Accel {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float FallingAccel  {: .copyable aria-label='Variables' }

___
### Falling·Speed {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float FallingSpeed  {: .copyable aria-label='Variables' }

___
### Height {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float Height  {: .copyable aria-label='Variables' }

Defines the height of a projectile. Height should be a negative value. Default is `:::lua -23`.
To make projectiles that remain at a perfectly stationary Height until collision, set FallingSpeed to `:::lua 0` and FallingAccel to `:::lua -0.1`.
___
### Homing·Strength {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float HomingStrength  {: .copyable aria-label='Variables' }

___
### Projectile·Flags {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### [ProjectileFlags](enums/ProjectileFlags.md) ProjectileFlags {: .copyable aria-label='Variables' }

Uses [ProjectileFlags](enums/ProjectileFlags.md) to define the projectile attributes.
___
### Scale {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### float Scale  {: .copyable aria-label='Variables' }

___
### Wiggle·Frame·Offset {: aria-label='Variables' }
[ ](#){: .alldlc .tooltip .badge }
#### int WiggleFrameOffset  {: .copyable aria-label='Variables' }

___
