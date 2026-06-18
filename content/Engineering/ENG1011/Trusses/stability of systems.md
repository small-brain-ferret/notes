---
publish: true
aliases:
  - stability
created: 2026-06-17T14:46:16.495+10:00
modified: 2026-06-17T16:00:35.809+10:00
---

> [!NOTE] Stability of a system
> Stability of a system requires more than having the same number of unknown reactive forces as available equilibrium equations (i.e. be [[Static determinancy|statically determinate]]).
>
> Generally systems are unstable if they have:
>
> 1. fewer than 3 reaction forces, or
> 2. reaction forces that are all parallel to each other, or
> 3. reaction forces that are all concurrent
>
> ![[Attachments/Screenshot 2026-06-17 at 14.48.02.png]]

> [!IMPORTANT]
> A body on supports can either be stable or unstable.
>
> Stable systems can either be [[Static determinancy|statically determinate]] or [[static indeterminancy|statically indeterminate]].

![[Attachments/Screenshot 2026-06-17 at 15.41.53.png]]

# Example

![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 07.56.46.png]]
Parallel reactions:

- There are 2 vertical reaction forces from the two roller supports at A and B
  - they are parallel
- Thus, there is no constraint horizontally.
- $F_C$ with a horizontal component causes the system to roll off the supports

Concurrent reactions:

- there are 3 reactions on the plate
  - 2 from pin A
  - 1 from weightless member B
- Thus, there is no reaction moment produced about that point
- $F_D$ will create a moment about the concurrency point and the body will rotate

![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 07.57.50.png]]
The $P$ load will cause the beam to rotate about point $A$ ($\sum M_a \neq 0$).
There, the system is unstable even though there are only 3 unknown reactions.
