---
Title: "BattleSnake"
Date: Mon, April 19, 2021
---
# _OVERVEIW_
**Over the course of the past few weeks, a teamate and I have been coding a Battle Snake.** We made the snake do all sorts of things, but our main problem was trying to get our snkae to avoid self and wall collision. We took a while, but figured that out and solved it by process of elimination and having an algorithmic mindset. In our team, my role was to figure out the algorithm which we would use for certain problems. I made the sequences for the self avoidance, the backtracking, and a few others as well. 
**Thinking algorithmically means to find a problem, and solve it in a step by step sequence, break it down, to the basic moves.** I learned that problem solving is difficult yet very simple. In our problems, we would break them down, and solve them bit by bit to reach the end goal.

# Problem

**We had to break this down from scratch, our snake only did random moves in the beginning. It would still loop on itself, crash into walls, and run out of health.
# Process
First we had to stop it from hitting walls, so we made this:
```javascript
if (!moves.canMoveUpWall(height, head.y)) {
			possibleMoves = possibleMoves.filter(dir => dir != "up")
		}
```

Here, we put this in, and basically it will see if the head.y+1 is equal to board height, and if it is, it will filter out 'up' as a possible move

# Key Takeaways

**Some key takeaways from this would be learning about algorthims to basically make an AI, and be able to break a problem down for easier processing.**

# What's Next

**If I could continue working on this build, I would improve it's capability to avoid trapping itself, as well as to avoid head to head collision via detection in all direction. For example, avoiding this:**

![snakeGif](https://exporter.battlesnake.com/games/92ba6b74-c971-4329-9568-83f6deeb904a/gif)
