# linux-screen-cheatsheet
Cheatsheet of commands to use for screen on linux.

## CORE COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| ``which screen`` | Check for screen |
| ``yum install screen`` | Install screen |
| ``screen`` | Run screen |
| ``screen -L`` | Run screen and log session |
| ``screen -ls`` | List screen sessions |
| ``CTRL+a , ?`` | Screen commands help, exit help menu with ``spacebar`` or ``enter`` |
| ``CTRL+a`` | Activate screen for commands |
| ``CTRL+a , c`` | Create a new window |
| ``CTRL+a , n`` |  Go to next window |
| ``CTRL+a , p`` | Go to previous window |
| ``CTRL+a , d`` | Detach from screen window |
| ``screen -r`` |  Reattach to screen window |
| ``CTRL+a , H`` | Create running log of session |
| ``CTRL+a , M`` | Check for activity |
| ``CTRL+a , _`` | Monitor for no output |
| ``CTRL+a , x`` | Lock screen session |
| ``CTRL+a , k`` | "Kill" screen (terminate) |
| ``exit`` | Close screen window session |

Sources: https://www.rackaid.com/blog/linux-screen-tutorial-and-how-to/#starting, 
https://www.computerhope.com/unix/screen.htm


