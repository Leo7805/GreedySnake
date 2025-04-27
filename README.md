# greedy_snake
- A extremely simple js &amp; html5 canvas based snake game. (贪吃蛇游戏)
- Author: Leo (geneleoc@gmail.com)
- [Demo](https://notus629.github.io/greedy_snake/)


# Basic Steps

1. **Draw the visible grid, initial positions of the snake and food**  
   - A grid with 30 horizontal and 30 vertical cells, each cell 15px in size (canvas total: 450x450px).  
   - Draw an initial snake with 5 body segments in the first row.  
   - Place the default food at the center of the grid.  
   - The top-left vertex coordinates of each cell represent its position.  
   - The snake consists of two parts: the **head** (with direction) and the **body**.  

2. **Make the snake move**  
   - Move the snake head based on keyboard arrow key inputs (using event listeners).  
   - Update the body to follow the head using this algorithm:  
     - Generate a new head (based on the old head’s direction).  
     - Generate a new body (discard the last segment/tail of the current snake array).  
     - Append the new head to the body.  

3. **Implement food consumption**  
   - **Collision detection**:  
     - Increase the snake’s length by adding a new tail segment.  
     - Remove the eaten food and generate a new random food item.  

4. **Automate movement** using `setInterval`.  

5. **Score calculation**.
