# Where Winds Meet — Team-Wide Buffs \& Debuffs (PvE Speedrun)

**Patch:** Global Version 2.1 · **Updated:** 2026-09-03

## The most important rule: two kinds of buff

**% damage bonuses all share one additive pool and dilute each other.**
Resistance shred sits in its own multiplier zone and doesn't.

|Your team's total % bonuses|A +8% debuff is really worth|A −10 res shred is really worth|
|-|-|-|
|+0%|+8.0%|+5% physical|
|+50%|+5.3%|+5% physical|
|+100%|+4.0%|+5% physical|
|+150%|+3.2%|+5% physical|

**The more buffs your team stacks, the more valuable resistance shred becomes.**
In a fully-buffed speedrun comp, a −10 resistance debuff can outperform a +8%
damage debuff outright.

*Penetration math:* `multiplier = 1 + (Pen − Res)/100` when Pen > Res. In PvE you
start \~100 effective penetration ahead, so you're **always** in this branch — no
breakpoint is reachable, and penetration is linear. A −N resistance shred is worth
`N / (200 + your pen)` in added damage of that type.

## The five damage types

A buff only boosts the type it names. Multiply by that type's share.

|Boost type|Multiply by|Why|
|-|-|-|
|**All damage**|**1.0**|Everything|
|**HP damage**|**\~1.0**|HP damage is what kills the boss|
|**Physical damage**|**\~0.65**|Physical share of a typical build|
|**Attribute damage**|**\~0.35**|Attribute share|
|**Qi damage**|**\~0.1 direct**|Real value is faster exhaustion, not raw damage|

*Split measured at 62.7% / 37.3% on a Bellstrike Splendor build.*

## Team-wide providers

|Path|What it does|Type|Zone|Est. team DMG|
|-|-|-|-|-|
|**Any (Bitter Seasons T6)**|−10 Phys Resistance, −6% Defense|Physical|Pen|\~+3.2%, undiluted|
|**Bamboocut Draught**|2% damage taken, all types|All|Additive|+2% → diluted, \~+1.0–1.3%|
|**Bamboocut Dust**|−10 Phys Resistance, +5% Qi|Physical + Qi|Pen / Additive|\~+3.2% undiluted, + break speed|
|**Bellstrike Splendor**|+10% Qi, Exhausted +8% HP, +8% Bellstrike|HP + Qi|Additive|+8% → possibly undiluted now|
|**Bellstrike Umbra**|−5% Defense, +5% DoT|Physical / DoT|Base / ?|\~+0.4% + DoT|
|**Silkbind Deluge**|+24% Team Damage, 12s/30s, Boss exhaust 10s → 12s|All|Additive|+24% → diluted, \~40% uptime|
|**Stonesplit Might**|+8% HP \& Qi|HP + Qi|Additive|+8% → diluted|
|**Stonesplit Strength**|−16 All Attribute Resistance|Attribute|Pen|\~+3.0%, undiluted|

## Why break speed matters more than the Qi number suggests

Qi damage is only worth \~0.1× as raw damage, but breaking the boss unlocks a
**10–12 second exhaustion window** where the boss can't fight back, takes **+10%
damage**, and most classes have skills that hit exhausted targets harder.

So Qi/break contributors (Soulbreak, Pale Petal, Thunder Shock's Qi half) should be
valued on **how much they accelerate breaks**, not on their damage number. Pale
Petal extending exhaust 10s → 12s is a 20% longer damage window — likely worth more
than its "no damage bonus" tooltip implies.

## Notes

* **% bonuses dilute, resistance shred doesn't.** See the table at the top. This is
the single biggest factor in ranking these.
* **Resistance shred ≫ defense shred.** −10 resistance ≈ +5% damage. −6% defense ≈
+0.8%. A "reduce defense by X%" tooltip is usually near-worthless.
* **Same-type resistance shreds stack near-additively.** Bitter Seasons + Phantom
Chime = −20 physical res. Gain is `N / (200 + pen)`, so at pen 33.7 the first −10
gives +4.28% and the second gives +4.10% — technically diminishing, practically
additive. **−20 res ≈ +8.6% physical, undiluted**, which beats any single % damage
debuff in this table once dilution is accounted for.
* **HP vs Qi ≈ 10:1** by developer valuation, from Divinecraft upgrade costs (both
upgrades cost 3 base: Fire→Cinder Ash adds +4% Qi, Poison→Viper's Fire adds +0.4%
HP; at 10:1 all four items land on two clean values). This undervalues Qi for
speedruns, where breaks gate damage windows.
* **Strayhunt (Bamboocut Draught)** is one of only two all-types effects in the
table. Small headline number, but it applies to 100% of damage instead of a share,
so it lands near +1% at typical bonus pools — comparable to a DoT or defense-shred
effect rather than to the resistance shreds. Zone assumed additive (unverified).
* **Patch note:** the Exhausted universal vulnerability and Qi Imbalance's bonus
vulnerability were moved into the Mechanism-Based DMG Boost zone "to mitigate
diminishing returns caused by multiplier dilution." That likely makes them
**stronger** (they no longer dilute in the general pool). Heavenquaker's
Soul-Shaken was split into base + applier-only portions.

## Sources

* [The Ultimate WWM Speedrun Guide](https://docs.google.com/document/d/1AYp2sWfTW3cID6Cbl1VI67mj1l3OUO3CASwx3mUAdy4/) — "the speedrun doc"
* [WWM In-depth Damage Formula](https://www.reddit.com/r/wherewindsmeet_/comments/1s2hm7g/wwm_indepth_damage_formula/) — full zone-by-zone formula, translated from Yoka's calculator sheet
* Ingame tooltips, testing, etc.

