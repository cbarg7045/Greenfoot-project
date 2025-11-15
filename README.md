# Greenfoot-project
Rescue1 Move Code
public class Rescue1 extends Actor
{
    /**
     * Act - do whatever the Rescue1 wants to do. This method is called whenever
     * the 'Act' or 'Run' button gets pressed in the environment.
     */
    public void act()
    {
        movePlayer();
    }
    private void movePlayer()
    {
        if (Greenfoot.isKeyDown("left"))
        {
            move(-2);  // move left
        }
        if (Greenfoot.isKeyDown("right"))
        {
            move(2);   // move right
        }
        if (Greenfoot.isKeyDown("up"))
        {
            setLocation(getX(), getY() - 2); // move up
        }
        if (Greenfoot.isKeyDown("down"))
        {
            setLocation(getX(), getY() + 2); // move down
        }
    }
}
