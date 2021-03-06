### Intent

Provide a mechanical means to resolve disputes where the possible set of outcomes is
negotiated in advance of a conflict’s introduction.

### Also Known As

Task Resolution

### Related Patterns

[:pattern:Contest Tree](/pattern/Contest Tree), [:pattern:Negotiated Contest](/pattern/Negotiated Contest)

### Motivation

The Generalized Contest design pattern structures contests is a way where the possible
set of outcomes is negotiated among the players before a conflict is even introduced.
Generalized Contests accomplish this goal by making available a set of allowable
actions that a character may undertake along with the possible results of those actions.
That is not to say that a game must specify all actions that a character may undertake,
only that those actions that are resolved through Generalized Contests must specify their
set of possible outcomes in advance of a conflict’s introduction. These “pre-
negotiations” essentially become part of the group’s “Social Contract”, the unspoken
but mutually understood code of acceptable behavior and other ground rules that
evolves within any cohesive group. Their adoption may be as simple as all players
agreeing to follow the rules as specified in a game’s text where the game provides a list
of Skills along with their effects. Any alterations or re-interpretations of those rules
demand a re-negotiation of the Social Contract. In this way, house rules arise that
adjust the rules as stated.

The specification of possible outcomes may thus come in any of the following forms:
 1.  Game text describing the possible set of outcomes of specific actions, such as individual Skill descriptions. (i.e., “The skill of opening locks can be used to unlock a single lock on a successful roll.”)
 2.  Game text describing actions in a general way, but specifying in detail the set of possible results of actions. (i.e., “An individual action cannot resolve a higher-level conflict, but it can result in any of the standard side-effects (player choice).”)
 3.  Prior player agreement that adopts a house rule into the Social Contract.
 
The important difference between this pattern and the Negotiated Contest design pattern is that the outcomes of Negotiated Contests are negotiated by the players after a conflict is introduced while those of Generalized Contests are negotiated before a conflict is introduced. Because Negotiated Contests require negotiation, they are highly flexibleand can adapt to virtually any kind of conflict. Generalized Contests lack this flexibility because they require generalizations that do not always fit the situation at hand. On the
other hand, Generalized Contests have the advantage of speed (on a contest-by-contest
basis) in that all negotiations have taken place prior to a conflict (usually far in advance
of the conflict).

A game using Negotiated Contest mechanics to decide contests can actually evolve into
one commonly using Generalized Contests through play. This happens when certain
character actions become so common that the Social Contract of the group accepts that
certain character actions always result in one of a small set of outcomes. Such cases
occur when players describe actions that others accept without question because the
validity of similar actions has been previously established through negotiation. Since
the negotiation pertaining to the action has already transpired, arguing against its
validity might violate the Social Contract without a re-negotiation. A debate opened up
on a character action might result in an alteration to the Social Contract so that a new
set of pre-defined outcomes is established for a class of action. The reverse is also true.
An action that would normally be resolved through a Generalized Contest might
occasionally be negotiated to take into account special circumstances. Because of the
malleability of Negotiated and Generalized Contests, the patterns are mirror images of
one another.

### Applicability

Use the Generalized Contest pattern when you:
 1.  Want to resolve some (possibly most) in-game conflicts without a negotiation phase.
 2.  Are willing to resolve conflicts that cannot be handled in a general way through Negotiated Contests.
The pattern is especially applicable to tactical games where players pit their gaming
skills against one another. The pre-defined nature of Generalized Contests allows
applicable conflicts to be resolved in an unbiased fashion. A big part of any such game
revolves around player knowledge of the available tactical options and their skill in
taking advantage of them.

Generalized Contests are also appropriate for games where the design goals include
creating lists of pre-defined Skills, Gifts, Flaws, and/or Handicaps. What this
essentially provides players is a collection of (hopefully) well thought-out generalized
win/lose conditions for a wide variety of character actions. Thus, a large body of
quality conflict material can be easily adopted by the simple act of consenting to view
the game text as authoritative.

Note that this consent is itself a negotiation among the players that adopts the game text
into the group’s Social Contract when playing the game. If some players later decide
that they don’t like some of the game rules as stated, they can either
 1.  Re-negotiate the generalized set of possible outcomes for specific actions and adopt these as house rules, or
 2.  Negotiate the set of possible outcomes for a single conflict after it has been introduced into play. 
In the first case, the negotiation merely replaces an old generalized rule with a new one.
So, it does not transform a Generalized Contest into a Negotiated Contest. However,
the second case does transform one into the other. So, you would be wise to explicitly
include some rules in your game to cover the possibility.

### Consequences

When negotiation enters the picture, the inherent subjectivity of the process can leave
some players feeling cheated in tactical games when they lose. Hard feelings between
players can result.

Generalized Contests quickly resolve common, often repeated conflicts. They also
allow a game author great influence over his setting and the kinds of conflicts that will
arise in his game. He is afforded this opportunity by virtue of the fact that he can
include as part of his game text descriptions of pre-defined contests in the form of
Skills, Gifts, and the like. These kinds of descriptions also provide players with myriad
examples of how the author envisions the game to be played.

If overused, the pattern can result in excessive amounts of text to cover all eventualities
(aka “rules-bloat”). It is probably a mistake to rely exclusively on Generalized Contests
to resolve all conflicts. This pattern is incapable of handling all possible special cases
that can arise in tabletop role-playing games. So, trying to force-fit the pattern to
handle more and more circumstances will only result in an ever-expanding set of rules
covering a never-ending stream of special cases.

### Implementation Concerns

In games where Negotiated Contests are not available, characters can attain goals only
through pre-negotiated rules. If a specific desired outcome is not adequately covered by
a rule, a problem arises. For example, the following exchange could occur in an
anthropomorphic game:

> **Game Master:** “A fierce thorn-wielding chipmunk with engorged cheeks blocks your frog’s path.”
> **Player:** “Grenouilles engages the rascal with a haughty croak.”

Depending on what the player wants to accomplish, a Generalized Contest may or may
not be appropriate. Suppose the player states his goal as follows:

> **Player:** “I punch the chipmunk in the stomach to make him spit out the purse he stole.”

It is unlikely that any game’s Generalized Contests include the possibility of forcing
chipmunks to spit out purses. The questions that must be answered by the system may
be something along these lines:
 1.  Does Grenouilles punch the chipmunk in the stomach?
 2.  Is the punch sufficiently forceful to cause the chipmunk to spit out what he has in his mouth?
 3.  Does the chipmunk actually have the purse in his mouth, or is it something else?

The first two contests may reasonably be covered by a game’s collection of Generalized
Contests. But the third question is unlikely to answerable in such a fashion. Many
games give the Game Master the responsibility of deciding these kinds of questions.
But, therein lay a problem. To put it simply, such a system gives players no real way of
accomplishing goals that fall outside the game’s set of Generalized Contests. Instead,
they must rely purely on the Game Master to give them what they want. In other words,
there is no negotiation phase taking place before a contest, so a successful outcome
might or might not result in what a player desires. So, our previous example might end
as follows:

> **Game Master:** “With a loud ‘Ooof,’ a shower of acorns spews out of the chipmunk’s cheek pouches.”

In a game without negotiated contests, a successful outcome to a contest does not
equate to the player gaining what he wants. A Game Master might unilaterally decide
to alter the actual effect. Similarly, a failed outcome does not equate to the player
losing, either:

> **Game Master:** “The chipmunk deftly avoids your attack and retains the contents of his mouth. But, you notice the glint of gold under a nearby bush.”

So, in a game lacking negotiated contests, the determination of the success or failure of
a character action has no absolute bearing on whether a player actually succeeds in his
goals. To avoid this problem, you can either
 1.  Implement rules that allow a Negotiated Contest to replace a Generalized Contest when appropriate, or
 2.  Implement rules that allow the results of your game’s Generalized Contests to feed into and influence higher-level Negotiated Contests. (See the [:pattern:Contest Tree](/pattern/Contest Tree) design pattern for advice on how to do this.)

If the game incorporates Negotiated Contests, the Game Master and the player would
negotiate the actual effects of a successful punch prior to rolling any dice (or drawing
cards, comparing numbers, or whatever). Such a negotiation might be as simple as
“Okay, if you win, then he’ll spit out the purse. If you lose, then Grenouilles trips,
allowing the chipmunk to scamper off into the underbrush. Is that acceptable?”

Assuming the agreement is acceptable to both players, a successful outcome would
result in something like the following:

> **Game Master:** “With a loud ‘Ooof,’ a shower of coins spews out of the chipmunk’s cheek pouches. With a gasp and a wheeze, the purse follows shortly thereafter.”

### Samples

Let’s create a simple Generalized Contest system for a game using skills.
The Skill Roll
A Skill Roll tells you whether your character can successfully use one of his skills. For
example, you will make a Skill Roll when your character tries to pick a lock, sneak
unheard, or train animals. To make a Skill Roll
 1.  Roll a d30.
 2.  Add your character's pertinent skill rank and appropriate attributes to your d30 score.
 3.  If the total equals or exceeds a set threshold, your Skill Roll succeeds. Unless otherwise stated, the threshold that any Skill Roll must overcome equals 15 plus the skill rank of any opposing agent.

The effects of success and failure for the most common uses of a skill are given in the
skill’s description. However, at times you will come across situations in which using a
skill seems appropriate to solve a problem, but the game text does not take into account
the specific circumstances facing your character. In such cases, it is perfectly
reasonable for you and your Game Master to discuss the situation and determine any
adjustments that need to be made to the roll. Perhaps more important, though, are that
you and your Game Master feel comfortable in negotiating the possible effects of
success and failure for your current situation. The effects of success and failure can be
wide ranging from those stated in the text.

### Known Uses

The Game Summaries section has extensive coverage of various Generalized Contest
systems, and it would be pointless to repeat them here. You should pay particular
attention to Dogs in the Vineyard (whose generalized “Raise” and “See” mechanics feed
into higher-level negotiated contests), and Rifts (to see how overusing Generalized
Contests can result in rules-bloat).

