# Ring-0-Fire :fire:

Research regarding common and developing ring-0 kernel driver and their local security complications
Author: Reed Huskey
Date: 2-11-2021

## Research Goals

As I start this well-treaded path, I want to personally understand the rings of privellege for Microsoft Windows and be able to apply my understanding to newly developed ring-0 drivers.

### Outline :construction:

* What is the Windows Kernel?
  * Ring-0 drivers?
  * Create my own driver?
* Anatomy of a kernel driver
* Past security flaws of these drivers
 * __Root-kit functionality__
   * Malware analysis of historic rootkits
* Security patches/implementations to eliminate flaws
* Application of my knowledge to Vanguard, Riot Games' anti-cheat ring-0 driver
* Report on my findings

> To-do information is found in the projects tab
> Any updates to version will be located there

### Purpose :eye:
The general purpose of this project is to learn more about the protection ring of Windows, specifically ring-0 drivers, and its relationship regarding security. (i.e. principle of least privllege etc.).

## Vanguard :closed_lock_with_key:

One of the better known and recent news-worthy kernel drivers is Riot Games' anti-cheat Vanguard. A semi-direct end goal would be to disect this driver and see if I could initiate some kind of local privllege escalation through it or impede its intended anti-cheat behavior.
