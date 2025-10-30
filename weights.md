# How the scoring works

Each slider gives a continuous value from 0 (left trait) to 100 (right trait).
For each clan we compute a raw score by summing its weighted contributions from every slider.
Then we compare that raw score to the maximum theoretical score that the clan *could* obtain (if every slider favored it fully)
and present the result as an **affinity percentage** for that clan (0–100%).
Each clan's affinity is independent, it shows how close the player is to that clan's ideal profile.

## Trais weights
- 0 → Irrelevant Trait

- 1 → Relevant Trait

- 2 → Important Trait

- 3 → Defining Trait

## Clans and weight table
Format: Clan → Trait 1 / Trait 2

|           Trait 1          |             Trait 2             | Banu Haqim | Brujah | Gangrel | Hecata | Lasombra | Malkavian | Ministry | Nosferatu | Ravnos | Salubri | Toreador | Tremere | Tzimisce | Ventrue |
|:-------------------------- |:------------------------------- |:----------:|:------:|:-------:|:------:|:--------:|:---------:|:--------:|:---------:|:------:|:-------:|:--------:|:-------:|:--------:|:-------:|
| Artistic                   | Scientific                      |     0/0    |   0/1  |   0/0   |   1/2  |    0/0   |    1/0    |    0/0   |    0/0    |   0/0  |   0/0   |   3/0    |   0/3   |    3/1   |   0/0   |
| Beauty                     | Utility                         |     0/1    |   0/0  |   0/1   |   1/2  |    1/1   |    1/1    |    2/2   |    0/3    |   2/0  |   0/1   |   3/0    |   0/1   |    3/1   |   0/1   |
| Book Smart                 | Street Smart                    |     2/1    |   2/2  |   0/3   |   2/1  |    0/1   |    2/1    |    1/2   |    1/2    |   0/3  |   1/2   |   1/1    |   3/0   |    1/0   |   2/1   |
| Cautious                   | Daring                          |     2/0    |   0/2  |   0/1   |   1/1  |    1/0   |    1/1    |    1/2   |    3/0    |   0/3  |   2/0   |   2/2    |   2/0   |    0/2   |   2/1   |
| Compassionate              | Dispassionate                   |     0/2    |   1/0  |   0/1   |   0/2  |    0/2   |    2/1    |    1/1   |    1/1    |   0/1  |   3/0   |   2/1    |   0/1   |    0/3   |   0/2   |
| Competitive                | Casual                          |     0/0    |   1/0  |   0/0   |   1/0  |    3/0   |    0/0    |    0/1   |    0/1    |   0/2  |   0/0   |   2/1    |   1/0   |    2/0   |   2/0   |
| Confident                  | Needs Reassurance               |     1/0    |   2/0  |   0/0   |   1/0  |    3/0   |    1/2    |    2/1   |    0/1    |   2/1  |   0/1   |   2/1    |   1/0   |    2/0   |   3/0   |
| Creative                   | Conventional                    |     0/2    |   1/0  |   1/0   |   1/1  |    0/1   |    2/0    |    1/0   |    0/2    |   2/0  |   1/0   |   2/1    |   0/2   |    2/0   |   0/2   |
| Decisive                   | Indecisive                      |     1/0    |   2/0  |   1/0   |   0/0  |    2/0   |    1/2    |    0/0   |    0/0    |   0/1  |   2/0   |   1/1    |   0/0   |    1/0   |   2/0   |
| Dependable                 | Flexible                        |     2/0    |   0/0  |   2/1   |   0/1  |    2/0   |    0/1    |    2/1   |    1/0    |   0/1  |   3/0   |   1/1    |   1/1   |    1/1   |   2/0   |
| Down to Earth              | Head in the Clouds              |     2/0    |   0/0  |   1/0   |   0/2  |    1/0   |    0/3    |    0/0   |    2/0    |   0/1  |   2/0   |   1/2    |   1/1   |    0/0   |   2/0   |
| End Justifies the Means    | Honorable Actions               |     0/3    |   0/0  |   0/1   |   2/0  |    3/0   |    1/1    |    1/0   |    1/0    |   0/0  |   0/3   |   0/0    |   2/0   |    2/0   |   2/0   |
| Fencing                    | Boxing                          |     2/1    |   0/2  |   0/2   |   0/1  |    0/2   |    0/0    |    0/0   |    0/1    |   0/0  |   0/0   |   0/0    |   0/0   |    0/1   |   1/1   |
| Flamboyant                 | Reserved                        |     0/1    |   1/0  |   0/2   |   0/1  |    1/0   |    1/1    |    2/0   |    0/3    |   2/0  |   0/2   |   3/0    |   1/2   |    2/0   |   2/0   |
| Free-spirited              | Disciplined                     |     0/3    |   3/0  |   2/0   |   1/1  |    1/2   |    1/0    |    2/0   |    0/1    |   3/0  |   1/2   |   2/1    |   0/3   |    1/0   |   0/2   |
| Guard dog                  | Alley cat                       |     2/2    |   0/2  |   2/2   |   1/1  |    0/1   |    0/1    |    1/0   |    2/0    |   0/1  |   2/0   |   1/0    |   0/1   |    1/0   |   0/0   |
| Heart                      | Head                            |     0/1    |   2/0  |   1/0   |   0/2  |    0/1   |    2/2    |    0/1   |    0/1    |   1/0  |   1/2   |   2/1    |   0/2   |    1/1   |   0/1   |
| Heart on Sleeve            | Poker Face                      |     0/1    |   2/0  |   1/0   |   0/0  |    0/2   |    1/0    |    0/1   |    0/1    |   1/0  |   0/2   |   2/2    |   0/1   |    0/1   |   0/2   |
| Hierarchy                  | Heterarchy                      |     2/0    |   0/2  |   0/2   |   2/0  |    1/0   |    0/0    |    0/1   |    1/1    |   0/3  |   0/1   |   1/0    |   3/0   |    0/0   |   2/0   |
| Hotel                      | Camping                         |     0/0    |   0/0  |   0/3   |   0/1  |    1/0   |    0/0    |    0/3   |    0/1    |   0/2  |   0/0   |   2/0    |   1/0   |    1/0   |   2/0   |
| Leader                     | Facilitator                     |     0/0    |   1/0  |   0/0   |   0/1  |    3/0   |    0/2    |    1/2   |    0/1    |   0/1  |   0/0   |   1/2    |   0/1   |    0/1   |   3/0   |
| Letter of the Law          | Spirit of the Law               |     2/2    |   0/1  |   0/0   |   0/1  |    1/1   |    1/1    |    0/1   |    0/0    |   0/0  |   0/1   |   0/0    |   1/0   |    0/0   |   1/2   |
| Library                    | Dojo                            |     1/2    |   1/2  |   0/1   |   3/0  |    0/0   |    1/0    |    0/0   |    0/0    |   0/0  |   1/0   |   1/0    |   3/0   |    1/0   |   0/0   |
| Likes Change               | Likes Stability                 |     0/2    |   3/0  |   2/0   |   1/0  |    0/1   |    1/1    |    0/2   |    0/2    |   3/0  |   0/1   |   1/1    |   0/2   |    2/0   |   0/2   |
| Likes to take things apart | If it ain't broke, don't fix it |     1/1    |   0/0  |   0/0   |   3/0  |    1/1   |    0/0    |    0/0   |    1/1    |   0/0  |   1/0   |   1/0    |   1/0   |    3/0   |   0/1   |
| Obedient                   | Rebellious                      |     2/0    |   0/3  |   0/1   |   0/1  |    1/1   |    0/2    |    0/2   |    1/0    |   0/2  |   0/1   |   1/1    |   3/0   |    0/1   |   1/0   |
| Paladin                    | Rogue                           |     2/1    |   1/0  |   0/1   |   0/1  |    0/2   |    0/0    |    0/1   |    0/3    |   0/3  |   2/1   |   0/1    |   0/1   |    0/1   |   0/0   |
| Peacemaker                 | Firebrand                       |     1/0    |   0/3  |   0/1   |   0/1  |    0/2   |    0/2    |    0/0   |    0/0    |   0/1  |   3/0   |   1/1    |   0/0   |    0/1   |   1/0   |
| Planner                    | Spontaneous                     |     1/1    |   0/1  |   0/1   |   2/0  |    2/1   |    1/2    |    1/0   |    2/0    |   0/2  |   2/0   |   1/1    |   1/0   |    1/2   |   2/1   |
| Playful                    | Serious                         |     0/2    |   1/0  |   1/2   |   0/1  |    2/1   |    2/1    |    1/0   |    0/1    |   2/0  |   0/2   |   2/0    |   0/1   |    2/1   |   0/1   |
| Spiritual                  | Skeptical                       |     2/0    |   0/1  |   1/0   |   2/1  |    2/0   |    1/1    |    3/0   |    1/0    |   1/0  |   2/0   |   0/1    |   1/2   |    1/1   |   0/1   |
| Tells the Truth            | Bends the Truth                 |     3/0    |   1/0  |   1/0   |   0/1  |    0/1   |    1/1    |    0/2   |    1/2    |   0/3  |   2/0   |   0/2    |   0/2   |    0/2   |   0/2   |
| Tense                      | Relaxed                         |     2/0    |   1/0  |   2/1   |   1/1  |    1/0   |    2/0    |    0/1   |    2/0    |   0/1  |   2/0   |   0/1    |   1/0   |    1/0   |   1/0   |
| Thinks Outside the Box     | Colors Inside the Lines         |     0/1    |   1/0  |   1/0   |   1/0  |    2/1   |    3/0    |    2/0   |    0/2    |   1/0  |   1/0   |   2/1    |   1/2   |    3/0   |   1/2   |
| Transparency               | Need-to-Know                    |     1/0    |   2/1  |   1/0   |   0/2  |    0/1   |    1/2    |    0/0   |    0/3    |   0/0  |   0/0   |   0/1    |   0/2   |    0/1   |   0/1   |
| Wolf Pack                  | Lone Wolf                       |     0/1    |   1/0  |   0/3   |   2/1  |    1/0   |    0/1    |    2/0   |    1/2    |   2/1  |   0/2   |   2/0    |   1/0   |    0/1   |   1/0   |
|       Sum of weights       |                                 |     65     |   53   |    50   |   60   |    62    |     64    |    53    |     57    |   55   |    58   |    74    |    60   |    60    |    61   |
