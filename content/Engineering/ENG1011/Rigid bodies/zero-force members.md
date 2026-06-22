---
publish: true
aliases:
  - zero-force member
created: 2026-06-18T11:12:01.412+10:00
modified: 2026-06-22T11:09:50.167+10:00
---

> [!NOTE] criterium
>
> - do not support any external loads or internal forces
> - provide rigidity and [[stability of systems|stability]] to the overall system by reducing deflection or [[buckling]]
> - simplify analysis if they are identified (reduces number of unknowns)

> [!NOTE] Rule 1 - zero force member
> If only 2 non-colinear members form a [[planar truss|truss]] joint, and no external load or [[Supports|support]] reaction is applied to the joint, then the two members must be zero-force.
>
> ![[Attachments/Screenshot 2026-06-18 at 11.19.09.png|200]]
> ![[Attachments/Screenshot 2026-06-18 at 11.19.32.png]]
> ![[Attachments/Screenshot 2026-06-18 at 11.45.56.png]]

> [!NOTE] Rule 2
> If 3 members form a [[planar truss|truss]] joint for which 2 of the members are collinear, then the third member is a zero-force member, provided there is:
>
> - no external force or [[Supports|support]] reaction, at the joint, that has a component that acts along the third member.
>
> Note: if there are more than 3 members on a joint, see if any of them are 0-force members, as they would not count as a force-contributing member.
>
> ![[Attachments/Screenshot 2026-06-18 at 11.58.57.png]]
> ![[Attachments/Screenshot 2026-06-18 at 11.59.11.png]]
> ![[Attachments/Screenshot 2026-06-18 at 11.59.22.png]]
