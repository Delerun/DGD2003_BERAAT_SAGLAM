School of the Dead – Game Design Document (GDD)

Game Title: School of the Dead  
Genre: Survival / Puzzle / Horror / Single Player  
Platform: PC / Unity  
Gameplay: The player must escape zombies in a floor with four corridors, solve puzzles to unlock a chest, and reach the exit.  
Duration: Maximum 15 minutes (countdown timer).

---

## 1. Game Summary

The player becomes trapped in the school at night. The floor has been quarantined and zombies are roaming the corridors. The player's objective is to unlock the chest, obtain the sword and the key, and escape by opening the exit door while avoiding zombies.

Next to the chest it says:  
“Only those who solve the code deserve the weapon.”

If the player cannot escape within 15 minutes, the game ends.

---

## 2. Story

Late at night, a student is left alone in the school. Just as they are about to leave the building, the electricity suddenly goes out and the entire floor is plunged into darkness.

Strange sounds begin echoing through the corridors.

An emergency message appears on the player's phone:

“Experiment failed. The virus has spread. The infected are behaving aggressively. Evacuate the building immediately.”

The player runs to the exit door, but it is locked.

Next to the door is an old security note:

“Emergency equipment is stored in the security chest.”

However, the chest is locked with a 3-digit code.

While exploring the floor, the player must avoid zombies and solve three different puzzles to discover the chest’s code.

But things get worse.

The building’s emergency security system has activated and the floor is about to be fully quarantined. Before the system completely seals the floor, the player must escape the building within 15 minutes.

The flashlight battery is limited, and it is the only light source because the phone battery is too low to use the phone’s flashlight.

---

## 3. Gameplay Mechanics

Movement: Walk with W/A/S/D, run with Shift.

Flashlight: Limited battery. Used to illuminate dark areas and see zombies and puzzles.

Puzzles: Solve three different puzzles to find the chest code.

Chest: Locked. When the correct code is entered, it opens and reveals a sword and a key.

Zombie AI: Zombies move using NavMeshAgent; if they see the player, they begin chasing.

Combat: After obtaining the sword, the player can approach zombies, fight them, or clear a path.

Door / Exit: Requires a key and cannot be opened without it.

Countdown Timer: 15 minutes. If time runs out, the player loses.

---

## 4. Floor Plan (Level Design)

Location: Kültür University – Floor 1  
Structure: 4 Corridors

Corridor 1 – Start Area:  
Starting point, Emergency Lockdown note, part of a flashlight can be found (low battery).

Corridor 2 – Puzzle 1:  
Encrypted board puzzle, a zombie wandering randomly, dark environment.

Corridor 3 – Puzzle 2:  
Symbol puzzle inside a classroom, hidden zombie, clue pointing to the chest room.

Corridor 4 – Puzzle 3 & Chest:  
Map/classroom clue, chest containing sword and key, final corridor with exit door (opens with key).

---

## 5. Puzzles

Puzzle 1 – Encrypted Board  
Clue: “2, 7, 4” (Order: 274)  
This is part of the chest code.

Puzzle 2 – Symbols  
Four different symbols and clues must be used to find the correct combination.

Puzzle 3 – Map Note  
A clue that reveals the chest is located in a classroom.

---

## 6. Zombie AI

Patrolling: Zombies walk randomly on the NavMesh.

Detection: If the player enters within 5 meters and is in the zombie’s field of view, the zombie begins chasing.

Chase Speed: 20% faster than the player.

Collision: If the player has no sword and gets touched, the player takes damage or loses the game.

---

## 7. Items and Their Functions

Flashlight: Limited battery, provides light.

Sword: Used to kill zombies, push them back, or clear a path.

Key: Required to open the exit door.

---

## 8. UI / HUD

Flashlight battery indicator  
Countdown timer: 15:00 → 0:00  
Inventory icons for sword and key  
“Game Over” or “You Escaped” messages

---

## 9. Sound and Atmosphere

Zombie growls and footsteps  
Ambient sounds in dark corridors  
Alarm and emergency system sounds  
Sound effect when opening the chest  
Sound effect when opening the door

---

## 10. Start Screen / Intro

EMERGENCY LOCKDOWN ACTIVATED  
FLOOR SEALING IN 15:00

A VIRUS HAS ESCAPED.  
ZOMBIES ARE ON THE LOOSE.

FIND THE SECURITY CHEST,  
GET THE SWORD AND KEY,  
AND ESCAPE BEFORE TIME RUNS OUT!
