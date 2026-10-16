# MG3
## Devlog

1. The default values for a float is 0.0f, int is 0, bool is false, and string is just an empty string: "".
2. The Update() method is a built-in Unity method, so it gets called in-engine. We dont actually need to call it ourselves. 
3. The TimerText class uses the timer to display how much time the player has remaining before the game ends. It knows when to display the game over screen due to the if-statement within the Update() method in the TimerText class. Every frame the game checks if the timer countdown is less than or equal to 0.0f, and only on the frame where these conditions are met does the game display the Game Over text. If you also look within the inspector, for the Text_Timer GameObject, the Timer Text component's Game Timer inspector field's value is set to the value of the Timer component within the Text_Timer GameObject, so the game counts down from that value and repeatedly runs Update() until it reaches less than or equal to 0.0f.

## Open-Source assets
- [Cat fighter spritesheet](https://opengameart.org/content/cat-fighter-sprite-sheet)
- [Food sprites](https://rcpstd.itch.io/pixel-food-pack)