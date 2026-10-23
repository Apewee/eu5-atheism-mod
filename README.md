# Age of Reason: Atheism (EU5 1.4)

A religion mod for Europa Universalis V 1.4 built around the Enlightenment idea that a
state can abolish the church that made it.

## What it adds

**Decision — Sponsor a Radical Thinker**

- Visible to **every Lutheran** country, from the start of the game. No law, no age and no
  other prerequisite is checked.
- Costs **6 months of trade and tax income** (the decision is greyed out until you can pay).
- Produces a radical thinker (a high-Administration character at your court) who founds the
  **Atheism** religion, and converts **your state, ruler and ruler's family** to it.
- Seeds an **Atheism movement** in your capital (20% of the city's population as supporters).
  The movement then spreads the religion through the population on its own, exactly the way the
  vanilla Lutheranism and Hellenism movements do, instead of the state converting every pop
  overnight.
- The AI never takes this decision.

**Movement — Atheism**

Mirrors the vanilla movements that carry Lutheranism and Hellenism through the population. The
decision seeds it in your capital with 20% of the city's population as supporters; from there it
spreads on its own to neighbouring locations, market centres and your capital, converting
Christian pops to Atheism. It grows faster in towns, cities, printing presses, universities and
scriptoria, and only starts seeding neighbours once 5% of a location is atheist.

**Religion — Atheism** (religion group: *Freethought*)

| Effect | Value |
|---|---|
| Base Clergy Power | **-500%** |
| Base Crown Power | **+100%** |
| Tolerance of heathen beliefs | **+4** |
| Tolerance of heretical beliefs | **+4** |

Atheism has no religious influence currency and does not want to convert, so its religious
aspects are adopted for **10 stability** instead (the vanilla price of aspects for non-Christian
faiths). It keeps your existing western-Christian visuals, and its map colour is a slate grey.

**Estate rename — Clergy → Free Thinkers**

The clergy estate is renamed only for countries whose state religion is Atheism. Every other
country still sees "Clergy". The rename is driven by a trigger inside the estate-name
customizable localization, so it applies everywhere the estate name is printed.

**Estate privileges — Free Thinkers**

All three grant the Free Thinkers **+5% estate satisfaction** and take 3 months to enact.

1. **Sponsored Free Thinking** — +5% Free Thinker satisfaction, +10% research speed,
   +50% Free Thinker power, at the cost of -2% tax efficiency.
2. **Cult of Reason** — +5% Free Thinker satisfaction, +0.10 monthly prestige,
   +10% stability cost efficiency, +0.005 global monthly prosperity, +40% Free Thinker power,
   -10% crown estate power.
3. **Civic Festivals** — +5% Free Thinker satisfaction, +2.5% target satisfaction for all
   estates, +1 tolerance of heathens, monthly drift towards Humanist, +25% Free Thinker power,
   at the cost of -2.5% tax efficiency.

**Estate privileges — nobility, burghers and commoners**

Two new privileges for each of the other three estates, available only to Atheist states:

| Estate | Privilege | Effects |
|---|---|---|
| Nobility | **Renunciation of Feudal Privileges** | -5% noble satisfaction, -25% noble power, +7.5% peasant satisfaction, +5% crown power, +5% tax efficiency |
| Nobility | **Secular Officer Academy** | +5% noble satisfaction, +10% noble power, +0.10 monthly army tradition, +5% land morale, -2% tax efficiency |
| Burghers | **Chartered Philosophical Societies** | +5% burgher satisfaction, +15% burgher power, +5% research speed, -10% Free Thinker power |
| Burghers | **Free Press** | +5% burgher satisfaction, +10% burgher power, +5 max literacy, +0.01 monthly literacy, +5% stability cost efficiency, -5% noble power |
| Commoners | **Abolition of the Tithe** | +10% commoner satisfaction, +10% commoner power, -30% Free Thinker power, +3% tax efficiency |
| Commoners | **Village Schools** | +7.5% commoner satisfaction, +5% commoner power, +5 max literacy, +3% research speed, -2% tax efficiency |

**Government reform — Supremacy of Reason**

Available to Atheist states from the Reformation age onwards:

- **Ability to declare religious wars** — unlocks the *War of Reason* casus belli against any
  country that still follows a revealed religion. It is a religious casus belli (`religious_casus_belli`),
  so it counts as a religious war for war enthusiasm, AI and peace treaties, and allows conquest
  of provinces.
- **+0.10 base research progress** every month.
- +5% stability cost efficiency.

The casus belli is removed again if the reform is repealed.

**Religious aspects (6)**

The Atheist faith has **three doctrine slots** and a pool of six aspects:

| Aspect | Effects |
|---|---|
| **Crack Down on the Old Ruling Class** | **-100% noble power**, **+25% burgher power**, **+25% commoner power**, monthly drift towards Humanist |
| **Natural Philosophy** | +5% research speed, +5 max literacy, monthly drift towards Innovative |
| **Popular Sovereignty** | -15% crown power, +15% burgher power, +15% commoner power, +10% stability cost efficiency |
| **Public Education** | +10 max literacy, +0.01 monthly literacy, +2.5% commoner satisfaction |
| **Secular Charity** | +5% commoner satisfaction, +0.005 global monthly prosperity, -0.005 global food decay, +10% stability cost efficiency |
| **Meritocratic Advancement** | +15% pop promotion speed, +10% burgher power, -10% noble power |

**Advance tree — 12 advances across ages 4–6**

Like every other faith, Atheism has its own branch of the age trees. Each advance is only visible
to a country whose state religion is Atheism, and the branch starts from a vanilla advance in the
same age.

*Age 4 — Reformation*
- **Reason over Revelation** (+1 tolerance of heretics, drift to Humanist)
- **Secular Administration** (+5% legislative efficiency, +10% crown power)
- **War of Pamphlets** (+5 max literacy, +0.01 monthly literacy)
- **Natural Law** (+5% research speed, drift to Innovative)

*Age 5 — Absolutism*
- **Public Academies** (+0.10 base research progress, +5 max literacy)
- **Civil Service** (+5% legislative efficiency, +10% burgher power)
- **The Secular Army** (+5% land morale, +2% discipline)
- **Republic of Letters** (+0.10 monthly prestige, +1 possible artist)

*Age 6 — Revolutions*
- **Reason Ascendant** (+10% stability cost efficiency, +2.5% satisfaction for all estates)
- **Scientific Agriculture** (production efficiency bonus, -0.005 global food decay)
- **Enlightened Administration** (+5% research speed, +10% crown power)
- **Revolutionary Republic** (stability investment, +10% commoner power)

## Installation

Copy the `atheism_mod` folder into your EU5 mod directory:

- Windows: `Documents/Paradox Interactive/Europa Universalis V/mod/atheism_mod`
- Linux (Proton): `.../steamapps/compatdata/3450310/pfx/drive_c/users/steamuser/Documents/Paradox Interactive/Europa Universalis V/mod/atheism_mod`

Enable it in the mod list, then start a campaign. The decision appears in the **Religious**
decisions tab for any Lutheran country.

## Compatibility notes

- `in_game/common/customizable_localization/estates.txt` is a full copy of the 1.4 vanilla file
  with one extra text block. Any other mod that also overwrites that file will conflict with the
  estate rename (load order decides the winner).
- The new content uses new files only (advances, aspects, reform, casus belli, privileges), so it
  should stack with most mods.
- The mod is authored against game version **1.4.***.

## Art credits

All illustrations are public-domain paintings and engravings from Wikimedia Commons, cropped and
converted to DDS. The complete source list with licensing is in [CREDITS.md](CREDITS.md); the
modding workspace's `art-src/` and `tools/build_art.sh` can regenerate every texture.

- *A Philosopher Lecturing on the Orrery* — Joseph Wright of Derby, 1766 (decision banner).
- *The Alchemist Discovering Phosphorus* — Joseph Wright of Derby, 1771 (Sponsored Free Thinking
  icon and mod thumbnail).
- *The Death of Socrates* — Jacques-Louis David, 1787 (Cult of Reason icon).
- *Fête de l'Être suprême* — Pierre-Antoine Demachy, 1794 (Civic Festivals icon).
- *The School of Athens* — Raphael, 1511 (Supremacy of Reason icon, Public Education aspect).
- *The Astronomer* — Johannes Vermeer, 1668 (Natural Philosophy aspect).
- *Serment du Jeu de Paume* — engraving by Isidore Stanislas Helman after C. Monnet (Popular
  Sovereignty aspect).
- *Liberty Leading the People* — Eugène Delacroix, 1830 (Crack Down on the Old Ruling Class
  aspect).
- *The Gleaners* — Jean-François Millet, 1857 (Abolition of the Tithe icon, Secular Charity
  aspect).
- *The Village School* — Jan Steen, c. 1670 (Village Schools icon).
- *The Syndics of the Drapers' Guild* — Rembrandt, 1662 (Chartered Philosophical Societies icon).
- *The Anatomy Lesson of Dr Nicolaes Tulp* — Rembrandt, 1632 (Free Press icon, Meritocratic
  Advancement aspect).
- *Oath of the Horatii* — Jacques-Louis David, 1784 (Secular Officer Academy icon).
- *Nuit du 4 août 1789* — bronze relief by Léopold Morice, Monument to the Republic, Paris
  (Renunciation of Feudal Privileges icon; CC0).
- *A printer's workshop* — engraving after Goussier, Wellcome Collection (Free Press icon;
  CC BY 4.0).
- *Prise de la Bastille* — Jean-Pierre Houël, 1789 (War of Reason casus belli icon).

The Atheism religion icon (torch of reason) is drawn for this mod as an SVG and exported to DDS.
