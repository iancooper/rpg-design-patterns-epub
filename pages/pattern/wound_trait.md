### Intent

Maintain injuries, physical or otherwise, as individual character traits.

### Also Known As

Not applicable

### Related Patterns

[:pattern:Endgame](/pattern/Endgame), [:pattern:Hit Points](/pattern/Hit Points), [:pattern:Rank](/pattern/Rank), [:pattern:Trait](/pattern/Trait), [:pattern:Trauma Gauge](/pattern/Trauma Gauge)

### Motivation

Games that individually track character injuries follow the Wound Trait pattern. In its
simplest form, the pattern does not provide any mechanical means of modifying a
character’s abilities when harmed. It merely describes the specific injuries a character
has sustained. If wounds need to impose some mechanical restrictions on characters to
satisfy design goals, they may certainly be augmented with other patterns, such as the
Rank, Hit Points, and Trauma Gauge patterns.

One reason a game designer might utilize wound traits is to enhance story potential. If
a player knows that a character has a gaping flesh wound on his left thigh, he can take
that into account when he narrates scenes involving the character. Games having
combat as their primary focus are often designed to simulate the “gritty realism” of
battle, and may use wound traits as one means of doing so.

Games about combat realism are likely to mix this pattern with the other injury tracking
techniques described above. They may also handle injuries far differently than games
centered on drama and story. In real life, wounds are a Bad Thing, so a game designer
seeking to accurately reflect real world conflicts will likely implement wounds as
having universally detrimental effects to those injured. The degrees to which various
wounds hinder characters may vary drastically depending on the location and severity
of the wound, but are unlikely to ever aid him.

On the other hand, a game targeting the telling of interesting stories might take a
different approach. First of all, wounds might be introduced only if they drive the
storyline forward in some fashion. For example, in a game based on the horror genre, a
storyline might progress more quickly and with greater believability if the protagonist, a
female Olympic track star, conveniently suffers a crippling leg wound so that the serial
killer can catch up with her and initiate the game’s climax. In such a game, a player
might willingly accept (or even suggest) this kind of a wound to increase dramatic
tension and push the plot forward. In so doing, the game might reward the player by
actually making it harder for the serial killer to slay the fleeing character. One good
way to reward players that accept disabilities to enhance storytelling is to use an
abstract meta-game mechanic. This maintains the “believability” of a story (in that it
doesn’t give wounded characters absurd physical enhancements) and at the same time
allows players more flexibility in their story options. Our horror game example might
provide players with “Plot Points” that they could spend in augmenting contest rolls
(see the Resource pattern). Our heroine would be physically hindered by her wound,
but the player would be rewarded with enough “Plot Points” to more than make up for
the injury’s debilitating effects.

### Applicability

The Wound Trait pattern is appropriate in games where you
 1.  Want to track individual wounds to increase combat detail or enhance story potential.
 2.  Are willing to accept the additional bookkeeping that recording individual wounds demands.
In games where wounding effects occur infrequently, the Wound Trait pattern is ideal.
True, the bookkeeping overhead is relatively high on a wound-by-wound basis. But, the
cost of tracking a small number of injuries during a game session is generally well
within the tolerance of most players’ sensibilities given the level of story potential the
pattern provides.

If you find the bookkeeping too high a price to pay, you might want to consider the [:pattern:Hit Points](/pattern/Hit Points) or [:pattern:Trauma Gauge](/pattern/Trauma Gauge) patterns instead. If you want to guarantee the survival of
characters until their roles are fully played out in a storyline, you should also consider
the [:pattern:Endgame](/pattern/Endgame) pattern.

### Consequences

Of all the health tracking patterns, the Wound Trait pattern provides the most detail. It
gives players reasonably clear views of their characters’ states of health, so scenes in
which injuries play a factor become easier to describe. However, overuse of the pattern
can bog down game flow with details that add little or no enjoyment to players. So, you
should use the pattern only to the degree that it supports the “mood” your game tries to
generate. Anything more will detract from your ultimate vision.

### Implementation Concerns

On its own, the wound trait pattern is conceptually very simple. If a character is
harmed, a note is made of the wound’s characteristics. However, if you need wounds to
provide some mechanical effect in contests, you need to find some other means to
accomplish this goal. Wound traits are commonly mixed with other patterns. For
example, wounds can be assigned a Rank to describe their severity. They can be
associated with a damage rating, which is subtracted from a character’s Hit Points or
added to a Trauma Gauge.

Some games provide tables that specify the effects of specific wounds. Wound tables
are usually based on the severity of a blow and can take into account factors such as hit
location and armor types. They can be as large as necessary to give the required level
of detail. Be warned, though, that table lookups like these can take significant amounts
of time to use.

### Samples

A game in which characters all play World War II infantry might rank individual
wounds according to their severity. The sum of the individual ranks could then be used
as a modifier to physical actions. After a difficult battle, a soldier might have the
following traits listed on his character sheet:

 | Wound                                 | Rank | 
 | -----                                 | ---- | 
 | Grazing bullet wound on left shoulder | 1    | 
 | Shrapnel wound on right thigh         | 2    | 
 | Bayonet wound on lower right abdomen  | 5    | 
 | Total                                 | 8    | 

### Known Uses

[:game:The Riddle of Steel](/game/The Riddle of Steel) has a variety of means to simulate injury. First, it has a Pain
attribute that is subtracted from a character’s dice pools on every combat round.
Damage is also delivered in the form of “Shock,” which reduces a character’s short
term combat effectiveness (a single round), but does not linger. Blood Loss also drains
Health, which can kill a character if Health drops to zero (see the [:pattern:Hit Points](/pattern/Hit Points) and
[:pattern:Attribute](/pattern/Attribute) patterns). However, perhaps the most important form of damage in the game
comes from “Wounds.” A wound is an injury delivered to a specific location. The
severity of a wound is determined by the Margin of Success of the attacker in landing
the blow. Its effects are determined by both its severity and its hit location according to
various tables. Each wound is unique with effects ranging from “Charlie Horse” to
“Death. Destruction of cerebellum. Really Messy.”

[:game:Rolemaster Fantasy Role Play](/game/Rolemaster Fantasy Role Play) uses “Hits” as its primary means of tracking physical
punishment (see the Hit Points pattern). But, it also uses wound traits to add flavor and
detail to combat. Attacks are made by rolling d100, adding the aggressor’s “Offensive
Bonus” (OB), subtracting the defender’s “Defensive Bonus” (DB), and looking up the
result on a table based on the weapon type used to deliver the blow. The tables take
into account the defender’s armor type. This lookup provides a damage rating, which is
subtracted from Hit Points, and a “Critical” rating ranging from A to E. The d100 is
rolled again and the result is looked up on a “Critical Strike Table” corresponding to the
weapon type used (Puncture, Slash, Heat, etc.). The second table lookup is based on the
criticality rating of the previous table lookup. The effects take into account whether the
defender must parry, cannot parry, is stunned, bleeds, or has other penalties and for how
long. The sheer volume of tables gives a wide variety of possible results ranging from
“Not very impressive” to “Blow turns hip to dust. Foe falls down. Attempts to stand.
Falls again and dies in 6 rounds.”

[:game:Universalis](/game/Universalis) treats injuries like all other traits. Wounds are purchased through the
expenditure of “coins,” which is the sole source of narrative power in the game (see the
[:pattern:Currency](/pattern/Currency) pattern). Wounds are simply traits that have the characteristic of reducing a
character’s effectiveness in some way. Multiple coins can be spent on any given wound
to augment its severity. Player must take the effects of wounds into account when
having characters perform actions. If they fail to do so to the other players’ satisfaction,
the “importance” of the wound counts against the character in conflict resolution. A
character can only be killed or otherwise permanently removed from a storyline by
spending a number of coins equal to the characters total “importance.” His importance
equals the sum of all importance values of all traits. So, a character that has been
inflicted with a wound is actually *harder* to kill than one that hasn’t been wounded,
even though the injury hinders his activity.

