## A first script, Hello World
CraftTweaker uses a purpose-built scripting language known as ZenScript.  
We'll start with a programming tradition, printing "Hello World!".  
First, open or create the `scripts` folder in the Minecraft game directory. If you're unsure where this is, run `/ct scripts` ingame to open it.  
Next, create a text file containing only `println("Hello World!");`, and save it in the `scripts` folder. Scripts can have any name, but the extension must be `.zs`.  
To apply changes made to scripts while the game is running, run `/reload`. 
Lastly, open the `crafttweaker.log` file in the game directory using any text editor. `craftweaker.log` can also be opened by running `/ct log` ingame. At the end of one of the lines will be `Hello World!`.

**Note**  
Each script is loaded on both the server and the client. Joining a server temporarily overrides the client's scripts with the server's. Useful for making changes on the server without players downloading scripts!  
Singleplayer has an integrated server, so
if you loaded a singleplayer world, you'll notice two `Hello World!`s, labeled `[SERVER]` & `[CLIENT]`. This is only a curiosity, your scripts will never need to know if they're running on the client or the server.

### Explanation  
Here's the code again  
`println("Hello World!");`  
The parentheses, `()`, make the line a function call. A function is a named piece of code that can be called (run) to perform a task. In between them are the arguments, in this case only `"Hello World!"`. It is a string, a sequence of characters enclosed in double quotes (`""`). The semicolon (`;`) ends the line. Every line of code must end with a semicolon.  