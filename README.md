Examination of whether or not it is possible to take two separately trained reinforcement learning models, and to combine them in such a way that:

1. The nets become strongly coupled
2. The combined net performs better at the combined task than the individual nets can when not coupled
3. The individual net results do not degrade during coupling

To do this, we create a Pong game where the vertical travel distance is large, and where the ball bounces off paddles at a random angle. We train one reinforcement model on the left half of the game screen, controlling the left paddle. Then we train a similar model using the right side of the screen and the right paddle. We then see whether it is possible to combine the trained models in such a way that the performance of each individual half does not degrade during combinatino, and where the two nets perform better at the combined task at the end.
