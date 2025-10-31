# How the scoring works

Each slider gives a continuous value from 0 (left trait) to 100 (right trait).
For each clan we compute a raw score by summing its weighted contributions from every slider.
Then we compare that raw score to the maximum theoretical score that the clan *could* obtain (if every slider favored it fully)
and present the result as an **affinity percentage** for that clan (0–100%).
Each clan's affinity is independent, it shows how close the player is to that clan's ideal profile.

## Trais weights
- 1 → Irrelevant Trait

- 2 → Relevant Trait

- 3 → Important Trait

- 4 → Defining Trait

## Clans and weight table
Format: Clan → Trait 1 / Trait 2

|           Trait 1          |             Trait 2             | Banu Haqim | Brujah | Gangrel | Hecata | Lasombra | Malkavian | Ministry | Nosferatu | Ravnos | Salubri | Toreador | Tremere | Tzimisce | Ventrue |
|:-------------------------- |:------------------------------- |:----------:|:------:|:-------:|:------:|:--------:|:---------:|:--------:|:---------:|:------:|:-------:|:--------:|:-------:|:--------:|:-------:|
| Artistic                   | Scientific                      |     1/1    |   1/2  |   1/1   |   2/4  |    1/1   |    2/1    |    1/1   |    1/1    |   1/1  |   1/1   |    4/1   |   1/4   |    3/2   |   1/1   |
| Beauty                     | Utility                         |     1/2    |   2/1  |   1/2   |   2/3  |    2/2   |    1/3    |    2/2   |    1/4    |   2/1  |   1/3   |    4/1   |   1/2   |    4/2   |   3/2   |
| Book Smart                 | Street Smart                    |     3/2    |   3/3  |   1/4   |   3/2  |    1/2   |    3/2    |    2/3   |    2/3    |   1/4  |   2/3   |    2/2   |   4/1   |    2/1   |   2/2   |
| Cautious                   | Daring                          |     3/1    |   1/3  |   1/3   |   1/2  |    2/1   |    1/2    |    2/3   |    4/1    |   1/3  |   3/1   |    2/3   |   3/1   |    1/3   |   3/2   |
| Compassionate              | Dispassionate                   |     1/3    |   2/1  |   2/2   |   1/3  |    1/3   |    3/2    |    2/2   |    2/2    |   2/3  |   4/1   |    3/1   |   1/2   |    1/4   |   1/3   |
| Competitive                | Casual                          |     1/1    |   3/1  |   2/2   |   3/1  |    3/1   |    1/1    |    1/2   |    1/2    |   2/3  |   1/1   |    2/1   |   2/1   |    3/1   |   3/1   |
| Confident                  | Needs Reassurance               |     2/1    |   3/1  |   2/2   |   2/1  |    4/1   |    2/3    |    3/2   |    1/2    |   3/2  |   1/2   |    3/2   |   2/1   |    3/1   |   4/1   |
| Creative                   | Conventional                    |     1/3    |   2/1  |   2/1   |   3/2  |    1/2   |    3/1    |    3/1   |    1/3    |   3/1  |   2/1   |    3/2   |   1/3   |    3/1   |   1/3   |
| Decisive                   | Indecisive                      |     2/1    |   3/1  |   2/1   |   1/1  |    3/1   |    2/3    |    1/1   |    2/2    |   1/2  |   2/1   |    1/1   |   1/1   |    2/1   |   3/1   |
| Dependable                 | Flexible                        |     2/1    |   1/1  |   3/2   |   1/2  |    3/1   |    1/2    |    3/2   |    2/1    |   1/3  |   3/1   |    1/3   |   2/2   |    2/2   |   3/1   |
| Down to Earth              | Head in the Clouds              |     2/1    |   1/1  |   2/1   |   1/3  |    2/1   |    1/4    |    1/1   |    3/1    |   1/2  |   3/1   |    1/3   |   2/2   |    2/2   |   3/1   |
| End Justifies the Means    | Honorable Actions               |     1/4    |   2/2  |   1/2   |   3/1  |    3/1   |    1/1    |    2/1   |    2/1    |   2/1  |   1/4   |    1/1   |   3/1   |    3/1   |   4/1   |
| Fencing                    | Boxing                          |     3/2    |   1/3  |   2/3   |   1/2  |    1/3   |    1/1    |    1/1   |    1/2    |   1/1  |   1/1   |    3/1   |   1/1   |    1/2   |   1/1   |
| Flamboyant                 | Reserved                        |     1/2    |   2/1  |   1/3   |   1/2  |    2/1   |    2/3    |    3/1   |    1/3    |   3/1  |   1/3   |    4/1   |   2/3   |    3/1   |   3/1   |
| Free-spirited              | Disciplined                     |     1/4    |   3/1  |   3/1   |   1/3  |    2/3   |    2/1    |    3/1   |    1/2    |   4/1  |   2/3   |    3/2   |   1/4   |    2/1   |   1/3   |
| Guard dog                  | Alley cat                       |     3/3    |   3/2  |   3/3   |   2/2  |    1/2   |    1/3    |    2/1   |    3/1    |   1/2  |   3/2   |    1/2   |   1/2   |    2/1   |   1/1   |
| Heart                      | Head                            |     1/2    |   3/1  |   3/1   |   1/3  |    1/2   |    2/2    |    1/2   |    1/3    |   3/1  |   2/3   |    3/1   |   1/3   |    2/2   |   1/2   |
| Heart on Sleeve            | Poker Face                      |     1/2    |   3/1  |   2/1   |   1/1  |    1/3   |    3/1    |    1/2   |    1/3    |   2/1  |   1/2   |    2/2   |   1/2   |    1/2   |   1/3   |
| Hierarchy                  | Heterarchy                      |     3/1    |   1/3  |   1/3   |   3/1  |    2/1   |    3/1    |    1/2   |    2/2    |   1/3  |   1/2   |    2/1   |   3/1   |    1/1   |   3/1   |
| Hotel                      | Camping                         |     1/1    |   1/2  |   1/4   |   1/1  |    2/1   |    1/1    |    1/4   |    1/2    |   1/3  |   1/1   |    3/1   |   2/1   |    2/1   |   3/1   |
| Leader                     | Facilitator                     |     1/1    |   2/1  |   1/1   |   1/2  |    4/1   |    1/3    |    2/4   |    2/3    |   1/2  |   1/1   |    2/3   |   1/2   |    3/2   |   4/1   |
| Letter of the Law          | Spirit of the Law               |     3/3    |   1/3  |   1/1   |   1/2  |    2/2   |    2/2    |    1/3   |    1/1    |   1/1  |   1/3   |    1/1   |   2/1   |    1/1   |   2/3   |
| Library                    | Dojo                            |     2/3    |   2/3  |   1/3   |   4/1  |    1/1   |    2/1    |    1/1   |    1/1    |   1/1  |   3/1   |    2/1   |   3/1   |    2/1   |   1/1   |
| Likes Change               | Likes Stability                 |     1/3    |   4/1  |   3/1   |   2/1  |    1/2   |    2/2    |    1/3   |    1/3    |   3/1  |   1/3   |    2/2   |   1/3   |    3/1   |   1/3   |
| Likes to take things apart | If it ain't broke, don't fix it |     2/2    |   2/1  |   1/1   |   4/1  |    2/2   |    1/1    |    2/1   |    2/2    |   2/1  |   2/1   |    1/1   |   2/1   |    4/1   |   1/2   |
| Obedient                   | Rebellious                      |     3/1    |   1/4  |   1/2   |   1/2  |    2/2   |    1/3    |    1/3   |    2/1    |   1/3  |   1/2   |    2/2   |   3/1   |    1/2   |   2/1   |
| Paladin                    | Rogue                           |     3/2    |   2/1  |   1/2   |   1/2  |    1/4   |    1/2    |    1/2   |    1/3    |   1/3  |   3/2   |    1/2   |   1/2   |    1/2   |   1/1   |
| Peacemaker                 | Firebrand                       |     2/1    |   1/4  |   1/3   |   1/2  |    1/3   |    1/3    |    1/1   |    1/1    |   1/2  |   4/1   |    1/1   |   2/2   |    1/2   |   2/1   |
| Planner                    | Spontaneous                     |     2/2    |   1/2  |   1/3   |   3/1  |    3/2   |    2/3    |    3/1   |    3/1    |   1/3  |   3/1   |    2/2   |   3/1   |    2/3   |   3/2   |
| Playful                    | Serious                         |     1/2    |   2/1  |   2/3   |   1/2  |    2/3   |    3/1    |    2/1   |    1/2    |   3/1  |   1/3   |    2/1   |   1/2   |    1/2   |   1/2   |
| Spiritual                  | Skeptical                       |     3/1    |   1/2  |   2/1   |   3/2  |    3/1   |    1/1    |    4/1   |    2/1    |   2/1  |   3/1   |    1/2   |   2/3   |    2/2   |   1/2   |
| Tells the Truth            | Bends the Truth                 |     4/1    |   2/1  |   2/1   |   1/2  |    1/2   |    2/1    |    1/3   |    2/3    |   1/4  |   3/2   |    1/3   |   1/3   |    1/3   |   1/3   |
| Tense                      | Relaxed                         |     2/1    |   3/1  |   3/2   |   2/2  |    2/1   |    3/1    |    1/3   |    3/1    |   2/3  |   3/1   |    1/2   |   3/1   |    2/1   |   2/1   |
| Thinks Outside the Box     | Colors Inside the Lines         |     1/2    |   2/1  |   2/1   |   2/1  |    3/2   |    4/1    |    3/2   |    1/3    |   3/1  |   2/1   |    3/2   |   2/3   |    3/1   |   2/3   |
| Transparency               | Need-to-Know                    |     2/1    |   3/2  |   2/1   |   1/3  |    1/2   |    1/4    |    2/3   |    1/4    |   1/2  |   1/1   |    1/2   |   1/3   |    1/2   |   1/2   |
| Wolf Pack                  | Lone Wolf                       |     1/2    |   2/1  |   1/4   |   3/2  |    2/1   |    1/2    |    3/1   |    2/3    |   3/2  |   1/3   |    2/1   |   2/1   |    1/3   |   2/1   |
|       Sum of weights       |                                 |     133    |   133  |   133   |   133  |    133   |    133    |    133   |    133    |   133  |   133   |    133   |   133   |    133   |   133   |