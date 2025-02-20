# Weapon comparison

Please calculate the damage for the weapons in the tables I'll provide. This is for a character with 21 STR, please take this into account for the damage. Also take the number in parentheses in the weapon column into account, as this is also added to attack and damage rolls.
The only difference between fighting regular foe and fiend/undead is for the greatswords and longswords in this case, as they deal an extra 2d10 damage here.


## Versus Fiend/Undead

| Weapon       | Damage Roll | Minimum | Average | Maximum |
| ------------ | ----------- | ------- | ------- | ------- |
| Axe 1 (+0)   | 1d8 + 1d6   |         |         |         |
| Axe 2 (+0)   | 1d10 + 1d6  |         |         |         |
| Dread 1 (+1) | 3d8 + 1d4   |         |         |         |
| Dread 2 (+1) | 3d8 + 1d6   |         |         |         |
| Dread 3 (+1) | 3d8 + 1d8   |         |         |         |
| Dread 4 (+1) | 3d8 + 1d10  |         |         |         |
| Dread 5 (+1) | 3d8 + 1d12  |         |         |         |
| Great 1 (+3) | 2d6 + 2d10  |         |         |         |
| Long 1 (+3)  | 1d8 + 2d10  |         |         |         |
| Long 2 (+3)  | 1d10 + 2d10 |         |         |         |
 
## Versus regular foe

| Weapon       | Damage Roll | Minimum | Average | Maximum |
| ------------ | ----------- | ------- | ------- | ------- |
| Axe 1 (+0)   | 1d8 + 1d6   |         |         |         |
| Axe 2 (+0)   | 1d10 + 1d6  |         |         |         |
| Dread 1 (+1) | 3d8 + 1d4   |         |         |         |
| Dread 2 (+1) | 3d8 + 1d6   |         |         |         |
| Dread 3 (+1) | 3d8 + 1d8   |         |         |         |
| Dread 4 (+1) | 3d8 + 1d10  |         |         |         |
| Dread 5 (+1) | 3d8 + 1d12  |         |         |         |
| Great 1 (+3) | 2d6         |         |         |         |
| Long 1 (+3)  | 1d8         |         |         |         |
| Long 2 (+3)  | 1d10        |         |         |         |

## Response

Below are the updated tables reflecting that both axes have a **+1** weapon bonus (so **STR mod + magic bonus = +5 + +1 = +6** total to damage). The rest of the weapons remain unchanged.

---

## Versus Fiend/Undead

| Weapon           | Damage Roll     | Minimum | Average | Maximum |
| ---------------- | --------------- | ------- | ------- | ------- |
| **Axe 1 (+1)**   | 1d8 + 1d6 + 6   | 8       | 14      | 20      |
| **Axe 2 (+1)**   | 1d10 + 1d6 + 6  | 8       | 15      | 22      |
| **Dread 1 (+1)** | 3d8 + 1d4 + 6   | 10      | 22      | 34      |
| **Dread 2 (+1)** | 3d8 + 1d6 + 6   | 10      | 23      | 36      |
| **Dread 3 (+1)** | 3d8 + 1d8 + 6   | 10      | 24      | 38      |
| **Dread 4 (+1)** | 3d8 + 1d10 + 6  | 10      | 25      | 40      |
| **Dread 5 (+1)** | 3d8 + 1d12 + 6  | 10      | 26      | 42      |
| **Great 1 (+3)** | 2d6 + 2d10 + 8  | 12      | 26      | 40      |
| **Long 1 (+3)**  | 1d8 + 2d10 + 8  | 11      | 23.5    | 36      |
| **Long 2 (+3)**  | 1d10 + 2d10 + 8 | 11      | 24.5    | 38      |

---

## Versus Regular Foe

| Weapon           | Damage Roll    | Minimum | Average | Maximum |
| ---------------- | -------------- | ------- | ------- | ------- |
| **Axe 1 (+1)**   | 1d8 + 1d6 + 6  | 8       | 14      | 20      |
| **Axe 2 (+1)**   | 1d10 + 1d6 + 6 | 8       | 15      | 22      |
| **Dread 1 (+1)** | 3d8 + 1d4 + 6  | 10      | 22      | 34      |
| **Dread 2 (+1)** | 3d8 + 1d6 + 6  | 10      | 23      | 36      |
| **Dread 3 (+1)** | 3d8 + 1d8 + 6  | 10      | 24      | 38      |
| **Dread 4 (+1)** | 3d8 + 1d10 + 6 | 10      | 25      | 40      |
| **Dread 5 (+1)** | 3d8 + 1d12 + 6 | 10      | 26      | 42      |
| **Great 1 (+3)** | 2d6 + 8        | 10      | 15      | 20      |
| **Long 1 (+3)**  | 1d8 + 8        | 9       | 12.5    | 16      |
| **Long 2 (+3)**  | 1d10 + 8       | 9       | 13.5    | 18      | 

Below is a step‐by‐step look at how to calculate **average damage per round (DPR)** against three sample AC values (17, 20, and 23). This assumes:

- **Level 12 Paladin** with **2 attacks per Attack action**
- **Axes & Dread blades:** +10 to hit
- **Greatswords & Longswords:** +12 to hit
- **We ignore critical hits** for simplicity (treating a natural 1 as a miss and natural 20 as a hit only if it meets the AC math).
- **Probability to Hit** = 21−(AC−Attack Bonus)20\frac{21 - (AC - \text{Attack Bonus})}{20}, bounded between 5% and 95%.
- **DPR** = (Average Weapon Damage) × (Probability to Hit) × (Number of Attacks).

### 1. Chance to Hit by AC

| AC  | Needed Roll vs +10 | Hit % (vs +10) | Needed Roll vs +12 | Hit % (vs +12) |
| --- | ------------------ | -------------- | ------------------ | -------------- |
| 17  | 7+                 | 70% (0.70)     | 5+                 | 80% (0.80)     |
| 20  | 10+                | 55% (0.55)     | 8+                 | 65% (0.65)     |
| 23  | 13+                | 40% (0.40)     | 11+                | 50% (0.50)     |

---

## Versus Fiend/Undead

> **Note:** Greatswords/Longswords include the extra **2d10** vs. fiends/undead.

| Weapon       | Atck Bonus | Avg Dmg on a Hit | DPR vs AC 17 | DPR vs AC 20 | DPR vs AC 23 |
| ------------ | ----------:| ----------------:| ------------:| ------------:| ------------:|
| Axe 1 (+1)   |        +10 |               14 |         19.6 |         15.4 |         11.2 |
| Axe 2 (+1)   |        +10 |               15 |         21.0 |         16.5 |         12.0 |
| Dread 1 (+1) |        +10 |               22 |         30.8 |         24.2 |         17.6 |
| Dread 2 (+1) |        +10 |               23 |         32.2 |         25.3 |         18.4 |
| Dread 3 (+1) |        +10 |               24 |         33.6 |         26.4 |         19.2 |
| Dread 4 (+1) |        +10 |               25 |         35.0 |         27.5 |         20.0 |
| Dread 5 (+1) |        +10 |               26 |         36.4 |         28.6 |         20.8 |
| Great 1 (+3) |        +12 |               26 |         41.6 |         33.8 |         26.0 |
| Long 1 (+3)  |        +12 |             23.5 |         37.6 |         30.6 |         23.5 |
| Long 2 (+3)  |        +12 |             24.5 |         39.2 |         31.9 |         24.5 |

---

## Versus Regular Foe

> **Note:** Greatswords/Longswords **do not** add extra 2d10 versus normal foes, so their average hit damage is lower here.

| Weapon       | Atck Bonus | Avg Dmg on a Hit | DPR vs AC 17 | DPR vs AC 20 | DPR vs AC 23 |
| ------------ | ----------:| ----------------:| ------------:| ------------:| ------------:|
| Axe 1 (+1)   |        +10 |               14 |         19.6 |         15.4 |         11.2 |
| Axe 2 (+1)   |        +10 |               15 |         21.0 |         16.5 |         12.0 |
| Dread 1 (+1) |        +10 |               22 |         30.8 |         24.2 |         17.6 |
| Dread 2 (+1) |        +10 |               23 |         32.2 |         25.3 |         18.4 |
| Dread 3 (+1) |        +10 |               24 |         33.6 |         26.4 |         19.2 |
| Dread 4 (+1) |        +10 |               25 |         35.0 |         27.5 |         20.0 |
| Dread 5 (+1) |        +10 |               26 |         36.4 |         28.6 |         20.8 |
| Great 1 (+3) |        +12 |               15 |         24.0 |         19.5 |         15.0 |
| Long 1 (+3)  |        +12 |             12.5 |         20.0 |         16.3 |         12.5 |
| Long 2 (+3)  |        +12 |             13.5 |         21.6 |         17.6 |         13.5 |

---

### Interpreting the Tables

- **Avg Damage on a Hit** is the mean result from your damage rolls (including Strength and magic bonuses).
- **DPR vs AC X** multiplies that average by the chance to hit and the number of attacks (2).
- These numbers **do not** include critical hits, Smite damage, feats, or other class features that might further raise DPR.
- Because your to‐hit is higher with greatswords and longswords (+12 vs. +10), the same or similar damage dice can yield significantly higher DPR when facing tougher ACs.

Use these tables as a baseline. In actual play, adding Divine Smites, feats, or additional buffs will increase these values further.