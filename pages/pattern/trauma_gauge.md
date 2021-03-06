### Intent

Provide a gauge for harmful effects on characters that hinders the use of related
attributes and abilities.

### Also Known As

Health Level, Weariness

### Related Patterns

[:pattern:Endgame](/pattern/Endgame), [:pattern:Hit Points](/pattern/Hit Points), [:pattern:Wound Trait](/pattern/Wound Trait)

### Motivation

Many role-playing games deal with exhaustion and mental or bodily injury. Games that
want to incorporate the incremental effects of various forms of injury, whether physical
or emotional, need some means to adequately simulate these effects without bogging
down the game mechanics with too much minutiae. Any role-playing game that assigns
a gauge to a character that somehow measures the character’s current state of health
(whether physical, spiritual, mental, or otherwise) and uses that gauge to lower the
effectiveness of related actions follows the Trauma Gauge pattern.

In its simplest form a Trauma Gauge has a value indicating the current degree of
wounding that a character has suffered. This gauge hinders the effectiveness of all
related abilities the character attempts. Often, a Trauma Gauge’s value is directly
subtracted from a character’s effectiveness although this is not a requirement of the
pattern. If a gauge measures the level of wounding a character has sustained and it has
some increasingly detrimental effect on a character’s actions as its value increases, it
follows the Trauma Gauge pattern. So, the greater the gauge value, the more the
character suffers from his injuries. Note that the pattern does not require that there be
any pre-defined level of injury at which the character “dies.” Depending on the game
requirements, a character could continue suffering greater and greater quantities of
trauma forever. In this way, the Trauma Gauge pattern greatly differs from the Hit
Points pattern. Of course, there is nothing preventing a game designer from “mixing in”
the Hit Points pattern by setting a limit to the amount of injury a character can suffer
before expiring.

Note that any gauge that measures a character’s state of “Health” is, for all practical
purposes, equivalent to any attribute measuring a character’s state of “Ill Health.” We
have chosen to call this pattern the Trauma Gauge pattern rather than the Health Gauge
pattern to highlight its differences from the Hit Points pattern. If you use an attribute
gauging the level of “Health” rather than “Injury,” you could easily state that a
character dies if his Health drops to zero. To have a Health attribute modify character
actions, then, you would first have to determine the level of damage sustained before
applying any adjustments (assuming a fully healthy individual applies a zero adjustment
to his abilities).

### Applicability

The Trauma Gauge pattern is appropriate in games where you
 1.  Need to incorporate rules dealing with injury and possibly death.
 2.  Want to simulate the incremental effects of injuries on character actions.
 3.  Are willing to accept the added calculation demanded by the pattern. 
If you find the arithmetical overhead too high a price to pay, you might want to consider
the Hit Points pattern instead. On the other hand, if you are willing to live with even
more bookkeeping to provide finer control over wounding effects, you should consider
using the Wound Trait pattern. Finally, if you want to guarantee the survival of
characters until their roles are fully played out in a storyline, you should consider the
Endgame pattern.

Please note that the Trauma Gauge, Wound Trait, and Endgame patterns are not
mutually exclusive. So, you might want to contemplate using some combination of
these patterns in your game rather than rely on any one pattern in isolation.

### Consequences

The Trauma Gauge pattern provides a gauge of a character’s current level of damage
and modifies the success of related actions based on this state of health. While this
sounds like an unquestionably Good Thing at first, the pattern does suffer from a
potential problem known as a “Death Spiral.” If a character is wounded in a game
incorporating the Trauma Gauge pattern, his abilities are henceforth reduced in potency.
This makes it easier for the character to sustain further injury, since any abilities he
might use to avoid future wounds are hampered. Sustaining more damage means the
character is even more susceptible to damage, etc. Unchecked, the pattern nudges a
character further and further along a spiral toward his death (or similarly catastrophic
result).

Generally, Hit Points are only modified and considered when a character sustains some
kind of damage. A Trauma Gauge, on the other hand, must be considered on every
character action to
 1.  See if it applies to the action, and,
 2.  Determine how much it affects the action.
Assuming characters perform actions more often than they sustain damage, the Trauma
Gauge pattern requires more overhead. Obviously, systems can be devised that reverse
this tendency. But, in most cases, Trauma Gauges require more overhead than Hit
Points.

### Implementation Concerns

If you use the Trauma Gauge pattern, you will want to make sure that the gauge is
applied uniformly across all related abilities so that it does not unfairly favor or hinder
any particular character actions. One way to do this is to ensure that all character
attributes lie on the same “scale” and all abilities use the same mechanics to resolve
conflicts. In other words, don’t make your character’s Strength attribute range from 1
to 4 while his Agility attribute has a range of 1 to 100. Similarly, don’t use a d12 for
Stealth checks and percentile dice for combat attacks.

To reduce the “Death Spiral” effect, some games apply an adjustment based on the
Trauma Gauge to character actions rather than use the gauge value directly. The
adjustments give a nod toward the debilitating effects of wounds without allowing them
to overpower a character too quickly. So, a Trauma Gauge value of 10 might translate
to a penalty of -2 and a value of 20 might translate to an actual penalty of -4.

Another option you might want to consider is to allow a player to “spend” his injuries
by accepting temporary (or permanent) flaws in exchange for a reduction in his current
Trauma Gauge value.

### Samples

Consider an “Office Cubicle” game that has an “Emotional Stress” attribute specifying
the current level of emotional injury that a character suffers. Conflict resolution is
performed using 1d10, adding pertinent abilities, subtracting “Emotional Stress” and
comparing the result to a threshold. The lists of traits and attributes include subjects
such as “Office Gossip,” “Backstabbing,” and “Political Correctness.” The more
meaningless paperwork piled on a character and the tighter his deadlines, the more
emotional damage he sustains. “Say, Wilson, do you have those TPS reports done,
yet?” Take 1 Stress. The character’s work ethic and productivity dwindle as greater
quantities of stress are piled on. Fortunately, at any time, a character can decide to
“spend” his stress points by indulging in some stress relieving activity:

 | Activity                                                       | Stress Relief | 
 | --------                                                       | ------------- | 
 | Jogging                                                        | -1 Stress     | 
 | Make fun of the Boss                                           | -1 Stress     | 
 | Vacation                                                       | -2 Stress     | 
 | Report Anonymous Tip to IRS about Company Accounting Practices | -5 Stress     | 
 | Quit Job                                                       | -5 Stress     | 
 | Writing a program to Embezzle Funds                            | -8 Stress     | 
 | Burning down the Office Building                               | -10 Stress    | 
 | Going “Postal”                                             | -10 Stress    | 

### Known Uses

In [:game:My Life with Master](/game/My Life with Master), minions have a “Weariness” attribute that increases as they
suffer injury. Weariness is directly subtracted from all actions except when
approaching “Connections.” Connections are NPC’s that enable minions to gain
“Love” which is an attribute that allows a minion to resist his Master’s commands.

[:game:The Riddle of Steel](/game/The Riddle of Steel) has a Pain attribute that is subtracted from a character’s dice pools
on every combat round. Pain accumulates as wounds are inflicted. The more Pain that
a character suffers, the less effective he is in combat and magic.

[:game:Sorcerer](/game/Sorcerer) has a Damage attribute (although it does not appear on the character sheet).
This attribute accumulates all damage inflicted upon a character and is directly
subtracted from all actions attempted by the character. Players have the option of
having their characters make “Will rolls” without penalty to temporarily forego some or
all of the effects of Damage. (This nicely sidesteps the death spiral effect.) The game
specifies the physical effects of different levels of Damage in comparison to a
character’s “Stamina,” such as “bruises,” “need stitches,” and “guts hanging out.” But,
interestingly enough, it doesn’t explicitly specify that a character can die from damage
alone. Death can arise when a character’s “Humanity” attribute drops to 0, but
alternatives to death exist as well depending on what Humanity actually means to a
given character.

[:game:The World of Darkness](/game/The World of Darkness) (Werewolf: The Apocalypse) gives each character a “Health
Level” attribute. After a successful attack is made, a separate damage roll determines
the amount of damage delivered. The game uses a dice pool for conflict resolution, so
each success on the damage roll indicates a point of damage. The Health Level attribute
has 7 possible values (8 if you count “Uninjured”). These are: Bruised (-0), Hurt (-1),
Injured (-1), Wounded (-2), Mauled (-2), Crippled (-5), and Incapacitated. Werewolves
regenerate damage at the rapid rate of one point per combat round, except for wounds
delivered by silver, fire, or other supernatural creatures.

