# sumScore v1.0

## OVERVIEW
sumScore is a simple, lightweight, and open source Unity Asset for adding scores to your game. 
It contains easy to set up Unity3d prefabs for displaying and storing scores. Includes option to 
save high score to PlayerPrefs. Uses the native Unity UI so you can easily change the look and 
feel of everything right in the editor. Licensed under MIT and CC0 so there are no worries on 
usage rights.

- Project Homepage: http://www.cyberlogical.com/sumscore/
- Repository: https://github.com/jerrydenton/sumScore

## SETUP
- Create a Canvas if there is not one in your scene already. [Create > UI > Canvas] in Hierarchy
- Copy one of the sumScore prefabs into your Canvas.
- (Optional) Adjust position on screen in the RectTransform component
- (Optional) Adjust colors, fonts, etc. to fit your game's style

## USAGE
The following public methods are available for manipulating the scores.

- **SumScore.Add(_int points_)** : Adds specified number of points to score
- **SumScore.Subtract(_int points_)** : Subtracts specified number of points from score
- **SumScore.Reset()** : Resets score to zero
- **SumScore.SaveHighScore()** : Saves player score as high score (if higher than current)
- **SumScore.ClearHighScore()** : Resets high score to zero

The following public properties are accessible

- **SumScore.Score** : Current player score. {get; protected set;}
- **SumScore.HighScore** : Current high score {get; set;}

**_Check 'SampleScene' for example of proper setup and usage_**

## OPTIONS
The following options are available on the 'sumScoreManager' component on each prefab

- *Initial Score* : Determine default score [int, def: 0]
- *Store High Score* : Save high scores to PlayerPrefs [bool, def: true]
- *Allow Negative* : Should we allow negative scores? [bool, def: false]
- *Field* : Just a link to the text field containing the player score. No need to change this one.
- *High Score Field* : Just a link to the text field containing the high score. No need to change this one.

## EXAMPLE
'SampleScene' contains examples of how everything works.

## PROJECT LICENSE
- The MIT License (MIT) - https://opensource.org/licenses/MIT
- Copyright (c) 2016 Jerry Denton

## OTHER ASSETS
- Fonts are from the awesome CC0 collection by asset creator Kenney - https://kenney.itch.io/
- License (Creative Commons Zero, CC0) - http://creativecommons.org/publicdomain/zero/1.0/

## CREATED BY
- Jerry Denton
- http://www.cyberlogical.com

### CHANGE NOTES
----------------------------------------------------------

- v 1.0
- Initial version

----------------------------------------------------------
