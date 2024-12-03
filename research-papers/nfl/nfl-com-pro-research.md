# NFL.com Pro Research

This document serves as documentation for how the NFL.com Pro data is structured and delivered. The impetus for this document was the discovery of some hidden snap count data in an official box score PDF that doesn't seem to be linked anywhere else.

## Film Room - Querystring Building

season = 4 digit year (ex 2024)
seasonTYPE = REG / POST / REG,POST
weekSlug = WEEK_#
gameId = GUID but you'll notice that only the first 8 characters change for games in a specific year
quarter = single INT where OT = 5
down = single INT
yardsToGoType = SHORT / MID / LONG

### Play Types

redzone = 0 or 1
goalToGo = 0 or 1
passPlay = 0 or 1
runPlay = 0 or 1
playType = play_type_rush / play_type_pass / play_type_sack / play_type_kickoff / play_type_punt / play_type_xp / play_type_field_goal / play_type_two_point_conversion

### Play Result

touchdown = 0 or 1
attempt = 0 or 1 (for pass attempts)
completion = 0 or 1 (for pass completions)
interception = 0 or 1
fumble = 0 or 1 (for rush attempts and fumbled snaps only)
fumbleLost = 0 or 1 (for rush attempts and fumbled snaps only)
rush10PlusYards = 0 or 1
reception = 0 or 1
sack = 0 or 1
