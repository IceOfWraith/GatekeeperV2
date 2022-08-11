# **Gatekeeper V2**

Welcome to the efforts of countless hours of learning and failed attempts at writing code that culminated into this project known as Gatekeeper! Originally this started out as a bot to bring CubeCoders AMP to Discord with support for only Minecraft, but has evolved into this encompasing project of providing support for any type of server AMP can run along with providing as many of AMPs core features inside of Discord.

Need Support or have questions? Please visit my Discord and post in the respective channels.
Come Join my Discord - **[Kat's Paradise](https://discord.gg/s5FnnsbJ)**


### **Requirements**
_________
- Python 3.1 or greater
- Pip 2.1 or greater
- Discord.py 2.0 or greater 
    - *Please visit: https://github.com/Rapptz/discord.py to install discord.py development version!*
- Cube Coders AMP License
    - *https://cubecoders.com/AMP*


## **Installation Methods**
___
### **Manual Instructions**
1. Open your command line: run `sudo apt-get install -y python3 pip && git clone https://github.com/Rapptz/discord.py && cd discord.py && python3 -m pip install -U .[voice]`
2. Create an AMP user for the Bot with `Super Admins` role.
3. Follow the instructions in `tokenstemplate.py` file -> [tokenstemplate.py](/tokenstemplate.py)
4. From Command Line run script `start.py` *(eg. `../Discord Bot/start.py`)*
    - Run the bot, it will finish installing the rest of the requirements.
5. See **Interacting with the Bot~**

### **AMP Instance Instructions**
1. Create an AMP user for the Bot with `Super Admins` role.
2. Create a new instance of GatekeeperV2 in a container. *(The container option can be found under `Configuration -> New Instance Defaults`)*
3. Configure the settings in the GatekeeperV2 Instance under the `Configuration -> Bot Settings`, click `Update`, then start the bot.
4. See **Interacting with the Bot~**
___

## **Interacting with the Bot**
*Channel ID and Channel Name are interchangable in commands*
**See [Commands](/COMMANDS.md) for a full list!**

__Setting up a NON-Adminstrator Role for the Bot__
- **TIP** - Use this if you want NON-Discord Admins to have the ability to interact with the bot*
- Use `/bot setup role_id` and the bot will add that role as the minimum required role to interact with the bot.
    - It does honor the role heirarchy set via `Discord -> Server Settings -> Roles`.


__Setting your AMP Console Channels__
- Use `/server console channel channel_id` and the bot will begin sending AMP Console messages to that channel. 
    - **TIP**: You can also send AMP Console commands through that Discord Channel to the Dedicated Server.


__Setting your AMP Chat Channels__
- Use `/server chat channel channel_id` and the bot will begin sending AMP Chat messages to that channel. 
    - **TIP**: You can also send Chat messages through that Discord Channel to the Dedicated Server.


__Setting your Whitelist Channel/Settings__
- Use `/bot whitelist channel set channel_id/channel_name`
    - *Optional*: Using the auto-whitelist feature, simply use the command `/bot whitelist auto whitelist true`
        - The Bot has a default wait time of 5 minutes. *(eg. `/bot whitelist waittime 5`)* **TIP**: You can set this value to `None` or `0`.
        - If the message was parsed successful they are added to the whitelist waitlist, after the timer is up they are whitelisted!.

______
## **Launch Args**
- `-token` - Bypasse tokens validation check. *(Mandatory for AMP Template Installations/Operations)*
- `-command` - Enable slash command print statements for user traceback.
- `-dev` - Enable development print statments. *(used for development)*
- `-debug` - Enables *DEBUGGING* level for logging. *(used for development)*
- `-discord` - Disables Discord Intigration *(used for testing)*
- `-super` - This leaves AMP Super Admin role intact, use at your own risk.    
___
### **Credits**
"**Thank You**" to everyone at CubeCoders Discord Server, especially *IceofWrath, Mike, Greelan* and everyone else in their discord.

"**Thank You**" to everyone over at Discord.py Discord Server, especially *SolsticeShard and sgtlaggy* for all the silly questions I kept asking about embed's and Hybrid messages!

___
### **Want to Support?**
*Visit my [Patreon](https://www.patreon.com/Gatekeeperv2)*