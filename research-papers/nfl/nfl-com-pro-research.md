# NFL.com Pro Research

This document serves as documentation for how the NFL.com Pro data is structured and delivered. The impetus for this document was the discovery of some hidden snap count data in an official box score PDF that doesn't seem to be linked anywhere else.

## Film Room - Querystring Building

season = 4 digit year (ex 2024)<br />
seasonTYPE = REG / POST / REG,POST<br />
weekSlug = WEEK_#<br />
gameId = GUID but you'll notice that only the first 8 characters change for games in a specific year<br />
quarter = single INT where OT = 5<br />
down = single INT<br />
yardsToGoType = SHORT / MID / LONG<br />

### Play Types

redzone = 0 or 1<br />
goalToGo = 0 or 1<br />
passPlay = 0 or 1<br />
runPlay = 0 or 1<br />
playType = play_type_rush / play_type_pass / play_type_sack / play_type_kickoff / play_type_punt / play_type_xp / play_type_field_goal / play_type_two_point_conversion<br />

### Play Result

touchdown = 0 or 1<br />
attempt = 0 or 1 (for pass attempts)<br />
completion = 0 or 1 (for pass completions)<br />
interception = 0 or 1<br />
fumble = 0 or 1 (for rush attempts and fumbled snaps only)<br />
fumbleLost = 0 or 1 (for rush attempts and fumbled snaps only)<br />
rush10PlusYards = 0 or 1<br />
reception = 0 or 1<br />
sack = 0 or 1<br />

### Presnap

qbAlignment = SHOTGUN / UNDER_CENTER / PISTOL<br />
rec_motion = 0 or 1 (for receiver motion)<br />

### Passing

targetLocation = OUTSIDE_NUMBERS / DOWN_SEAMS / BETWEEN_HASHES
