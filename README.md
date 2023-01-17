Roleplaying Game Dice: Statistics and Gameplay
================

## Introduction

In 2015, I won a contest from [Evil Hat
Productions](https://www.evilhat.com/home/) as part of the Evil Hat
Street team. My prize was an hour long conversation with members of the
Evil Hat team on a subject of my choosing. My friend
[John](https://github.com/owendl/rpgaday2020/blob/master/29-ride-DO.md)
and I got on a call with Sean Nittner and Fred Hicks to discuss game
design. In our conversation, Sean brought up the balance of agency
versus experience in roleplaying games. The interaction of these two
concepts with game dice mechanics in two different roleplaying game
systems is the subject of this paper.

### Agency

Agency decscribes the control the players have over the game and the
characters destiny (Reference for more explanation:
[link](http://game-wisdom.com/critical/player-agency-game-design-narrative).
Games with high agency give players a greater degree of control of the
world and what happens. In these games, the players are exerting their
will on the game, primarily via their characters. Other narrative
options are available in some games (Assets in Cortex, narrative
declaration in Fate) but as these do not participate with the dice
mechanics they are not considered.

### Experience

By contrast experience is the world of the game imposing its will on the
characters. Low agency games In the context of the original
conversation, experience was framed as the inverse of agency. Thus a low
agency game, could be considered as high experience and vice versa.

A high Experience game then sees players with less control over the game
world through the dice.

## Drama and Dice

### Powered by the Apocalypse

Powered by the Apocalypse games (PbtA) utilize a dice mechanic first
popularized by the game Apocalypse World by Vincent Baker. The governing
dice mechanic could not be any simpler, roll two six-sided dice (2d6)
and add a stat, typically ranging from -1 to 2. A 6 or lower (6-) is a
failure, 7-9 is a partial success and a 10+ is a full success. What is a
success and variations thereof can change game to game but the core
mechanic stays the same.

Below is a table of the potential results from this mechancic and their
proportion of possible roles (ignoring stat modification).

|     2 |     3 |     4 |     5 |     6 |     7 |     8 |     9 |    10 |    11 |    12 |
|------:|------:|------:|------:|------:|------:|------:|------:|------:|------:|------:|
| 0.028 | 0.056 | 0.083 | 0.111 | 0.139 | 0.167 | 0.139 | 0.111 | 0.083 | 0.056 | 0.028 |

Frequency of Results of 2d6

A few notes on these results:

-   42% of PbtA rolls are a failure on the dice (6-)
-   42% of PbtA rolls are only a partial success on the dice (7-9)

### Fate

The Fate roleplaying system builds off of the FUDGE roleplaying system
dice mechanic, where four FUDGE/Fate dice (4df) are rolled and then the
combined results are totaled. These dice are also six-sided but two
faces are blank (0), two have a “-” sign (-1) and two faces have a “+”
sign (+1). Thus the range of values for a 4df roll is -4 to 4. Beyond
the dice themselves, players add skills to the rolls, typically ranging
from 0 to 5.

|    -4 |    -3 |    -2 |    -1 |     0 |     1 |     2 |     3 |     4 |
|------:|------:|------:|------:|------:|------:|------:|------:|------:|
| 0.012 | 0.049 | 0.123 | 0.198 | 0.235 | 0.198 | 0.123 | 0.049 | 0.012 |

Frequency of Results of 4df

Consideration of failure or success based on the dice is more difficult
to determine because there is not standard target number. However, in
the context of control, it is easy to predict the outcome of a roll
based on the skill used. Almost two out of three rolls, 63%, of Fate
dice rolls are -1, 0 or 1. Thus, most rolls are approximately the value
of the character’s skill.

### Savage Worlds

### Comparing Different Dice

![](dice_spread_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->

The two additional lines are of two normal distributions
$N(0,4), N(0,9)$. These provide rough estimations of the distributions
of the two different dice mechanics.

### Agency and Experience: a personal thoughts

In Fate games, the outcomes are more predictable, the dice clustering
around zero. Extreme results are possible but very unlikely. Powered by
the Apocalypse games have a flatter spread, extreme results entering the
realm of plausible. And failure is guaranteed almost half of the time.

I remember thinking during our conversatoin with Fred and Sean that I
play Fate for the agency and Powered by the Apocalypse games for the
experience. I didn’t think much about it until recently when I began to
ask myself what the shape of the dice looks like. It makes sense that
the game was called Apocalypse World, the dice are very much the world
acting on you. Contrast that with Fate, where the outcome is actually
within your grasp (and even more so when considering Fate points).

I find Fate games really sing with a lighter, more playful tone while
the best PbtA games lean into the seriousness their names imply. Neither
game is really better than the other, each provides its own tenor and
style to games.

### Update Jan 2023

I have recently come across a variation on the Apocalypse World dice
mechanic called advantage and disadvantage. A player with advantage
(something in the narrative favoring them) a player gets to roll three
six-sided dice (3d6) and sum the the two highest dice (a roll of 2,4,6
becomes a result of 10). If a player rolls with disadvantage (something
in the fiction is acting against them) they again roll 3d6 but sum the
two lowest dice (a roll of 2,4,6 becomes a result of 6). I was curious
to look at how this affected the dice distributions. Below is the
distribution of normal Apocalypse World (pbta), with advantage
(pbta_adv) and disadvantage (pbta_dis).

![](dice_spread_files/figure-gfm/unnamed-chunk-7-1.png)<!-- -->

Intuitively it makes sense that advantage or disadvantage modified the
mean of the distributions. What I found more interesting was that the
variance also changed drastically, moving into close to the variance of
a high agency game like Fate.
