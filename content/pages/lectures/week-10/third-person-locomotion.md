---
title: "Third person movements" 
---

Disable the Firstperson GameObject by un-checking it in the inspector. Drag the third person prefab into your Hierarchy. Create a new script inside the scripts/audio folder called `ThirdPersonLocomotionSound`. Use the same code from your first person script but remove the capability to measure footstep frequency. Make the AudioClip variables match this:

```c#
public AudioClip[] FootstepSFX;
public AudioClip[] LandSFX;
public AudioClip[] JumpEmote;
public AudioClip[] LandEmote; 
```

Also make sure you have four functions to play each sound. 

Add an AudioSource called LocomotionSource to Ellen. If you just added it to the Thirdperson it wouldn't follow Ellen. Place both sources where you think the sound should emanate from in the scene. Uncheck play on awake for both sources. 