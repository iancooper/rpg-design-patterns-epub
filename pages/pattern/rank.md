### Intent

Allow players to customize their characters by assigning individualized proficiency
ratings to abilities.

### Also Known As

Attribute Level, Skill Level

### Related Patterns

[:pattern:Skill](/pattern/Skill), [:pattern:Skill Tree](/pattern/Skill Tree), [:pattern:Template](/pattern/Template), [:pattern:Trait](/pattern/Trait)

### Motivation

The Rank pattern individually associates a proficiency rating to all (or some) of a
character’s abilities. The ratings are usually numeric in nature, but the pattern does not
demand this. For example, ratings of “novice,” “competent,” “professional,” and
“expert” could be applied instead.

In games using the Skill or Skill Tree patterns, character abilities are selected from predefined lists of abilities. Those patterns assume that characters will gain proficiency in
their skills as play progresses. Games using the Traits pattern may also decide that
allowing varying degrees of proficiency in abilities is appropriate. However, none of
these patterns specifies the granularity of player control over his character’s abilities.
Some games uniformly raise the proficiency of all (or many) abilities based on a single
character rating (see the Level pattern). Others allow ability rankings to be customized
on an ability-by-ability basis. Games allowing individual ability ratings to be controlled
by the player exhibit the Rank pattern.

The primary reason to provide this fine a degree of control is to give players tools to
better achieve their visions of their characters’ personas. Ability ranking systems often
force players to trade off their characters’ proficiency rankings in some abilities to
increase them in others. Since no ability rating can be raised without some cost to other
abilities, a player must determine his character’s priorities. From the choices that are
made, the player’s aspirations are, to some degree, revealed.

For some players, a primary motive for favoring a ranking system is to attain better
“realism” than they could if they played a game lacking this feature. After all, real
people possess skills at various levels of ability, so why shouldn’t characters? Such
people often find systems that use a uniform “level” for all abilities to be too confining.

### Applicability

Use the Rank pattern if you
 1.  Are using the Trait, Skill, or Skill Tree patterns in your game design.
 2.  Want to provide players a great deal of control over ability proficiencies.
 3.  Are willing to accept the bookkeeping overhead needed for players to individualize their character’s ability rankings.
The Rank pattern demands additional accounting work from the players, since every
ability must somehow be associated with a ranking. If you do not want to require the
additional overhead demanded by the Rank pattern, you might want to consider the
[:pattern:Level](/pattern/Level) pattern instead.

### Consequences

The Rank pattern gives players a good amount of input into their character designs. It
forces the player to make trade-offs between the rankings of his character’s various
abilities, allowing him to gain greater proficiency in one or more abilities at the expense
of others. The player’s priorities are shown through his decisions. Allowing players to
customize their characters to the extent allowed in the Rank pattern does have its costs,
though. Additional bookwork of keeping track of a ranking for each skill is required at
the very least.

### Implementation Concerns

When you use the Rank pattern, your key decision will lie in how to trade off the
proficiencies of one ability for those of another. Some games using this pattern make it
more and more expensive to raise a particular ability’s rank as it increases, but this is
not a requirement of the pattern. If you use a fixed cost scheme to raise ranks, you will
either have to decide on some way to limit the amount a character can spend in a skill or
have some viable means of dealing with very large rank values. Of course, you could
just make all ranks extremely expensive so that a player can only raise a few ranks at
most, but that would conflict with the primary reason to use the Rank pattern in the first
place: to allow players to customize their characters.

Of course, any kind of “cost” to raise a rank implies that a player has some resource
from which to draw to increase his character’s rankings (see the [:pattern:Resource](/pattern/Resource) pattern).
Many games use a resource tied to how “seasoned” the character is, or how much
“experience” he has accumulated by overcoming obstacles. However, there is no
reason you must tie yourself to an experience based resource to control ability ranks,
should you decide some other measure is appropriate for your game. Nor should you
necessarily constrain your game to the traditional mode of having players raise
character ranks by drawing from resources under their control. It is not too hard to
envision a game whose focus is on inter-player negotiation that prohibits players from
spending their own resources on their own characters’ ability ranks. Such a game might
require players to negotiate for other players’ resources to increase their own characters’
skill and trait ranks.

Assuming you have players assign ranks by drawing from some resource, you need to
think carefully about what ability ranks can be assigned from a given resource. For
example, suppose you design a game with the following features:
 1.  Characters possess a fixed number of attributes and a variable number of skills.
 2.  It uses a classic “attribute value + skill rank + die roll” resolution system.
 3.  Any given attribute applies to a broader range of situations than any given skill.
 4.  Players spend “Experience Points” to gain skill ranks.

Let’s suppose you also decide to allow players to spend “Experience Points” on gaining
attribute ranks. By doing so, you may have just created a subtle problem. Attributes
are used in a wider variety of situations than skills. So, attribute ranks are more
valuable than skill ranks. It behooves players to spend more of their resources on
raising their attribute ranks than in raising their skill ranks. The degree to which this is
true depends on the disparity between the number of attributes and the number of skills.
Essentially, you have created an exchange rate between attributes and skills which
favors attributes over skills. A shrewd player will favor his character’s attributes at the
sacrifice of skills. If you are not very careful in designing your ranking system, skills
may inadvertently become completely irrelevant. One of the best solutions to this
dilemma is to avoid it entirely: associate one resource with attribute ranks and an
entirely independent resource with skill ranks. Do not allow *any* form of exchange or
interaction between these two resource pools. Note that the same argument holds
regardless of the kinds of gauges to which ranks are applied (Traits, Attributes, Skills,
Handicaps, etc). If the ranks of one kind of gauge are more valuable than those of
another, you need to keep their resource pools separate.

If you plan on giving characters a large number of ranked abilities, you have another
concern. That is how you are going to balance flexibility in your system with the
bookkeeping overhead it requires. Do you assume all skills are equally hard to learn
(and gain ranks) or do you make some skills easier to learn than others? Making the
cost structure uniform for all skills would lower the complexity of your system (and
reduce bookkeeping), but takes away a powerful design tool you could use to balance
one skill against another. For example, in many fantasy games, big swords and axes are
often preferred over daggers and other small weapons. This is because big weapons
presumably deliver more damage due to their “superior” size. But, if you allow
characters to gain proficiency in small weapons at a fraction of the cost of big weapons,
you can make weapon choice an arbitrary decision. Players using such a system are
much more likely to choose their weapons based on character concept and other
aesthetic reasons rather than from concerns about effectiveness.

Be aware that the Rank pattern’s bookkeeping overhead can quickly balloon out of
control by poor design decisions with very little tangible benefit to the game overall.
This can happen if you decide to make the costs of gaining a rank variable depending on
circumstances. You could decide that the cost of gaining a rank depends on a die roll.
If a player is “lucky,” he suffers only half the cost than if he is “unlucky.” Alternately,
you could make the first rank gained within a “game month” to cost less than the
second, third, or fourth ranks gained in the same month. While the incremental costs of
these kinds of rules seem low at first, the cumulative costs can become prohibitive and
painfully obvious in other circumstances. For example, suppose a player needs to work
up a powerful character from scratch. What are his character’s costs going to be for
gaining all of his various skill ranks? If the costs to gain a rank are dependent on
factors other than skill difficulty and rank, he will have to devote time to rolling dice or
performing table lookups individually on *every* skill rank his character gains. Gaining a
rank of 10 on a single ability would then require 10 separate calculations! If, on the
other hand, your game’s rank costs depend only on difficulty of an ability and the
desired rank, then a single calculation can be performed for every ability to determine
the costs.

### Samples

Melissa is working up a new character for a cartoon-based game. She has decided to
create a clumsy dim-witted dog named “Caper” that has turned to a life of crime as a cat
burglar for the simple reason that he wants to steal cats. However, Melissa wants Caper
to be particularly bad at his job. She wants him to accidentally make noises at
inconvenient times, by stepping on squeaky floorboards or knocking over vases, and
have a habit of breaking things, the more valuable the better. Melissa wants Caper to
have some useful abilities too. She wants Caper to be able to put on a skimpy black
mask to hide his identity in a “if-I-put-on-my-glasses-you-can’t-tell-I’m-Superman”
kind of way. Caper will also have a Cat Burglar’s Almanac that he carries around in a
burlap bag from which he gets all of his “brilliant” ideas. Finally, she wants Caper to
be able to climb through upper-story windows through the use of a grapnel hook and
rope that he also keeps in his bag. After all, what good is a cat burglar if he can’t throw
a grapnel through a second-story window to the sound of breaking glass? The game
Melissa is playing allows her to assign both positive and negative ranks to skills, with
negative ranks being as expensive as positive ranks, but making a character atrociously
(and, hopefully, humorously) un-adept at the skill. (The game gives rewards based
solely on whether you make other players laugh : 1 Character Point per chuckle.) The
cost to gain a given rank in a skill equals the skill rank value multiplied by itself. To
start, Melissa has 50 “Character Points” to spend on skills and decides to use them in
the following way:

Stealth: -4 (costing 16 “Character Points”)\\
Reading Comprehension: -2 (costing 4 “Character Points”)\\
Disguise: 5 (costing 25 “Character Points”)\\
Climbing: 2 (costing 4 “Character Points”)\\
Picking Locks: 1 (costing 1 “Character Point”)

### Known Uses

[:game:Dungeons & Dragons v.3.5](/game/Dungeons & Dragons v.3.5) has a list of 45 basic skills to which all characters have
access (see the Skill pattern). Players spend “skill points” to raise their ranks in their
skills. The number of skill points a player has to spend is determined by both his
character’s class (see the Class pattern) and level (see the Level pattern). “In class”
skills can be raised to a maximum of the character’s level + 3 at a cost of 1 rank per
skill point. “Cross class” skills can be raised to a maximum of only half the “in class”
maximum at a cost of 2 skill points per rank.

[:game:GURPS](/game/GURPS) (Basic Set) has a list of approximately 174 skills, depending on how they are
counted (see the Skill pattern). “Bonus points” can be spent on raising skill “levels,”
which actually corresponds to the Rank pattern (rather than the Level pattern). Skills
are segmented into Mental and Physical categories and are rated as “Easy,” “Average,”
“Hard,” or “Very Hard.” The cost to raise a rank is dependant on the difficulty of the
skill and the character’s attributes of DX (for Physical skills) and IQ (for Mental skills).

[:game:HeroQuest](/game/HeroQuest) has “abilities” that are essentially traits (see the [:pattern:Trait](/pattern/Trait) pattern). Very broad
abilities are known as “keywords” that act as templates (see the Template pattern), and
represent all abilities common for an occupation, culture, religion, and the like. Each
ability has a “rating” that is essentially a number between 1 and 80, but is represented
by four distinct levels of “mastery,” each of which is subdivided into values of 1 to 20.
So, a rating of 44 would be represented as 4 at mastery level 2 (20 x 2 + 4 = 44). In
conflict resolution, a contestant with a higher mastery level in the pertinent abilities has
a distinct advantage over those of lower mastery level.

[:game:The Pool](/game/The Pool) uses “traits” to describe character abilities (see the Trait pattern). In this
game, a trait is associated with a numerical value that allows a player to add dice to his
character’s “Dice Pool” (see the Dice Pool design pattern) in resolving conflicts
involving the trait. The more dice used in resolving a conflict, the more likely a
character will succeed. The cost of increasing the “bonus” for a trait is exponential,
though, and this cost is exacted from the same pool that feeds dice to all conflicts in
which the character participates (see the Currency pattern). So, there is tension between
building up a character’s long-term Traits and his likelihood for short-term success in
all endeavors. Success in any conflict results in the player choosing between adding a
die to his pool or controlling the outcome of the attempted action. Failure indicates that
the character loses whatever dice were “gambled” on the attempt (see the [:pattern:Resource](/pattern/Resource)
pattern).

[:game:Rolemaster Fantasy Role Playing](/game/Rolemaster Fantasy Role Playing) has 158 skills segmented into 47 skill categories
(see the Skill pattern). The game gives players “development points” to spend on
improving their character’s skills, which are awarded when the character gains levels
(see the [:pattern:Level](/pattern/Level) pattern). The cost to raise a skill is uniform across all skills within a
category. The actual costs also depend on the character’s class (see the [:pattern:Class](/pattern/Class) pattern)
and are variable depending on whether it is the first, second, or third skill rank gained in
the skill at the current level. Depending on the skill and class, a character may be
completely unable to raise a rank in a skill, or may be able to raise only one or two
ranks per level. For example, a Bard character has a cost of 2/7 in the Subterfuge :
Stealth skill category. This means that when he gains a level, the Bard can raise any
Subterfuge : Stealth skill (Hiding, Picking Pockets, Stalking, Trickery) by one rank by
expending 2 DP’s (development points). He can raise the same skill another rank by
spending 7 DP’s. He cannot raise the same skill any more ranks until gaining another
level.

[:game:Universalis](/game/Universalis) allows players to apply “traits” to characters through the expenditure of
“Coins,” such as “Loves Children” or “Blacksmith” (see the Trait pattern). Even a
character’s name is a trait in Universalis that must be purchased through coin
expenditures. The more coins that are spent on a particular trait, the greater its
“importance” rating. The overall “importance” of a character to the story is the sum of
all of the “importance” ratings of each of his individual traits. To “kill” a character or
otherwise entirely remove him from play, a number of coins must be spent equal to his
overall importance. Note that this does not work as a form of “Hit Points” (see the Hit
Points pattern for details), because a wound caused to a character by one player can
actually allow a player to add the trait “Wounded on Left Thigh +2” to the character by
spending 2 coins, which actually makes it *harder* to remove the character from play.

