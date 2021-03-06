### Intent

Provide a means for players to design their characters’ attribute values by trading them
off against one another.
{{ :pattern:point-spend-attributes.png}}

### Also Known As

Not Applicable

### Related Patterns

[:pattern:Attribute](/pattern/Attribute), [:pattern:Random Attribute](/pattern/Random Attribute), [:pattern:Resource](/pattern/Resource)

### Motivation

Many games assign Attributes to their characters so that various important game aspects
of the character can be gauged. The reasons for assigning Attributes to characters is
sufficiently covered in the Attributes design pattern, and will not be repeated here.
However, the process by which attributes values are set is another important
consideration, because attributes can play a key role in any game incorporating them.
The Point Spend Attributes design pattern does this by providing a resource (or
resources) to a player that he can spend in setting his character’s attribute values. So, a
player must make character-defining decisions about what is important to him. This
process allows a player to quickly and efficiently design a character that he will
personally enjoy playing.

### Applicability

There are essentially two schools of thinking in terms of character generation:
 1.  Character generation should focus on creating characters that players are excited about playing,
 2.  Character generation should focus on creating characters that seemingly existed in the game world prior to being adopted by a player.
Use the Point Spend Attributes pattern when your design goals favor the first option
over the second. If you prefer the second alternative, you might want to consider
setting attributes by using the Random Attribute pattern instead.

### Consequences

From the viewpoint that a character is fundamentally a tool by which a player interacts
with the game world, character generation boils down to nothing more than a process by
which that tool is constructed. Character generation, then, should be geared toward
creating as effective a tool as possible as efficiently as possible. In this light, it is not
difficult to see the benefits provided by the Point Spend Attributes pattern. With little
fuss, it accomplishes essentially three goals simultaneously:

 1.  It gives players great flexibility in designing the characters they envision,
 2.  A Point Spend system does not inadvertently favor one character over another (as can happen when attribute values are randomly generated),
 3.  It is fast and simple, so it does not unduly extend character generation.

The drawback to a Point Spend system is that it is obvious that the whole process is
contrived to allow a player to design a character rather than discover one. Techniques
that randomly generate attribute values and other characteristics are often viewed by
players as more of a discovery process, since the player has no real control over what is
generated (or his control is at least reduced). The problem with random character
generation is that players will often spend inordinate amounts of time rolling dice to
“discover” a character they would like to play. The Point Spend Attribute pattern cuts
through all that unnecessary red-tape and allows a player to get the character he wants
to play right away.

### Implementation Concerns

In using the Point Spend Attributes pattern, you should keep it simple. One good way is
to create a resource for players to spend solely on setting the values of a group of
attributes. The best way to do this is to have one point of the resource equate to one
attribute point (see the Currency pattern for reasons why this is so).

Some games allow the attribute resource to be spent on other things as well (such as
gifts, skills, or traits). However, doing so can be problematic because this forces the
game designer to find some equitable balance between an attribute point and everything
else the resource can buy. Otherwise, the choice of what to buy will really be no choice
at all since the player will naturally want to gain the most advantage out of the resources
you give him.

For example, attributes are often used as adjustments to skill rolls and attributes are
generally much fewer in number than skills. In this case, a single attribute point is
worth more than a single skill rank because a single attribute is applied to multiple skill
rolls. This difference in value increases as the number of skills provided by the game
increases. So, a shrewd player will favor attribute points over skill ranks if the same
points are used to buy both.

Even worse, if you inadvertently allow a gift that was bought to be re-exchanged for the
original resource at a different rate, you have a potentially horrid situation where a
player can essentially generate however many resource points he wants. (Don’t laugh!
At least one version of [:game:GURPS](/game/GURPS) has this problem.) If you want to allow players to buy
skills, gifts, and other characteristics, there is nothing wrong with creating a separate
resource devoted to that end. Isolating subsystems from one another in this way solves
the problems mentioned above.

The Point Spend Attribute pattern has one more potential problem. Players that
min/max their Characters tend to distribute their points similarly in games that use Point
Spend Attributes, at least for similar archetypes. For example, suppose you design a
fantasy game with attributes of both Strength and Magic where Strength is good for
hand-to-hand combatants and Magic is good for spell-casters. If you use the Point
Spend Attribute pattern, then almost any min/max-er creating a Wizard character will
focus his points on the Magic attribute. You will rarely, if ever, see a Wizard with a
high Strength and low Magic even though this variant may be interesting from a role-
playing perspective. Depending on the importance of these attributes on the mechanics
of the game, you may actually end up seeing exactly the same distribution of points
from character to character.

You may decide this is not a big issue for your game design, though, since it may take a
few campaigns and several years for any single group of players to figure out the
nuances of your game sufficiently to fall into predictable spending patterns. On the
other hand, you may decide that the problem is important enough to mitigate. One
potential option is to have some random factor included in the number of points to
spend. This would prevent characters of similar archetypes from always having exactly
the same distribution of attribute points. But, this solution inherently starts different
characters off on different footings, which will likely seem unfair to some players.
Another option is to make your attributes conflicted in some way (see the Conflicted
Gauge pattern) so that higher attribute values are good in some ways, but are
detrimental in others. That way, each player will have to weigh the good and the bad
for each point he spends. Different players will make different decisions when
confronted with real choices like these. Conflicted Gauges require careful scrutiny by
players, though, so making your attributes conflicted will tend to slow down character
generation. In short, no solution is perfect.

### Samples

Suppose we create a “Top Gun” style game. We plan on making dog fights a big part
of the game. To that end, we give the pilot characters attributes such as “Reflex,”
“Eyesight,” “G Forces,” “Recklessness,” and “Courage,” all of which range in value
from 1 to 10. Conflict resolution uses a number of d10 equal to a skill rank and
compares the rolled values against an attribute value. Any numbers that come up
greater than or equal to the pertinent attribute value are counted as successes and the
side with the greatest number of successes wins the contest. So, low attribute values are
better than high attribute values. The attribute values are set by spending a resource of
20 points named “Attribute Bonuses.” All attributes start at a value of 10, but every
“Attribute Bonus” spent lowers an attribute value by one to a minimum of two.

### Known Uses

[:game:Ars Magica](/game/Ars Magica) gives characters eight primary attributes of “Intelligence,” “Perception,”
“Strength,” “Stamina,” “Presence,” “Communication,” “Dexterity,” and “Quickness.”
The game has two ways to set attribute values. One of them is a Point Spend Attributes
system. Players are given 7 points to spend on attribute values. The costs of a given
value depend on a table lookup. Players can earn more points to spend by accepting
negative attribute values in some areas.

[:game:GURPS](/game/GURPS) characters are designed using a system based purely on “Character Points.”
Character Points are a resource that players spend to customize their characters. The
same resource is used to purchase attribute values as is used to purchase Skills,
“Advantages,” and other characteristics. Further, more “Character Points” can be
obtained by accepting various “Quirks” and “Disadvantages.” The cost of any given
Attribute value is variable and depends on a table lookup.

[:game:Hero System 5t Edition](/game/Hero System 5t Edition) uses eight primary attributes. Their values are specified by
having players spend “Character Points” and the costs vary from attribute to attribute.
The genre of game, whether heroic or super-heroic, determines the number of points
distributed to players to generate their characters.

[:game:Inspectres](/game/Inspectres) characters have four primary attributes: “Academics,” “Athletics,”
“Technology,” and “Contact.” “Normal” characters (i.e. humans) are given 9 “dice” to
distribute to these four attributes, but all must lie in the range of 1 to 4. (Although the
resource name of “dice” implies that dice are rolled to determine the attribute value, the
resource is really just a Point Spend system where one resource point equals one
attribute point. The Attribute value determines how many dice are added to conflict
rolls when the attribute applies, and this is where the resource name originates.)
“Weird” characters (i.e. werewolves, vampires, etc.) are given 10 “dice” to spend, with
each attribute value falling into the range of 0 to 10. The game allows only one weird
agent per game.

[:game:Shadowrun](/game/Shadowrun) characters have eight primary attributes, which are set by spending from a
pool of Attribute Points. The size of the pool is determined by the priority at which a
player sets his attributes for his character in comparison to skills, magic, race, and
resources. So, the more a player emphasizes attributes over other factors, the more
attribute points he gets to spend in designing his character. A player may increase this
pool size further by accepting “Allergies”, which are handicaps of various sorts.

