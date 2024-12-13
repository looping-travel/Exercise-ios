# Intro
Welcome to FlyLooping.com IOS design and coding exercise!

Read on…

# Exercise description
This is a tennis tournament; for a match, the rules are as follows:
- `Points` in a game are counted as: `0`, `15`, `30`, `40`
- A `game` is won when a player has `40` points and wins one more point, i.e. there is no _deuce_ or _advantage_.
- A `set` is won when a player reaches `6` games, i.e. there is no _tie-break_.
- A `match` is won when a player has 2 `sets`

In order to help the umpire score a match betwen player *X* and player *Y*, you will provide him with an app:
- with which he can enter the names of the players
- that displays the current score with the following information:

| Name                | Sets | Games | Points       |
|:-------------------:|:----:|:-----:|:------------:|
| <Name of player *X*> | 0-3  | 0-6   | [0/15/30/40] |
| <Name of player *Y*> | 0-3  | 0-6   | [0/15/30/40] |

- when a `point` is won, the umpire just has to press on the winning player name. the score is adjusted accordingly
- when a `match` is won, another screen is displayed:
*Winner: <Name of winning player>*
- during the match, the app will send the scoring (player names with scores, as per the above table) to a remote REST service (so as to display the score on TV channels)

## Optional features
- the umpire may make a mistake; provide him with a facility (that you will design) to correct the last point
- the app will keep all scorings from all matches it's been used in

# What we expect
- An IOS app written in swift with SwiftUI that helps the umpire with the scoring.
- The app will run on a simulator or actual IOS device.
- It will adapt to different IOS device screens (from iPhone Mini to Max Pro)
- You will implement the REST scoring service. The service can just print out the scores it receives
- The code will be versioned under _git_, on _GitHub_
