![Image](https://cdn.discordapp.com/attachments/1007859633400053863/1010219528325709915/lunars-mod-sys.jpg)
# djs-moderation-system
A DJS moderation system that every server needs, full with ban, kick, and timeout commands. This command also includes logs so you can track what your mods do!

## Dependencies:
-  mongoose => `npm i mongoose`
-  chalk => `npm i chalk@4.1.2`
-  dotenv => `npm i dotenv`

# Instructions:
1) Place the command into your commands folder.
2) Create a new folder in the bot root direcatory and name it "schemas", and than place the schema in there.
3) Change all the paths to the right ones if needed.
4) Place the event into your events folder.

# MongoDB Connection:
- be sure to add this to your ready.js file.
```
    // Add this to the top of the file
    const { connect } = require('mongoose')
    const chalk = require("chalk")
    
    // Add this to your ready.js file
    await connect(MONGO_URI)
      .then(() => {
        console.log(chalk.yellow(`✅ >>> Successfully connected to MongoDB!`));
      })
      .catch((err) => {
        console.log(err);
      });
```

# Preview

### ModLogs for kicks
![image](https://user-images.githubusercontent.com/91988772/185661831-8bd66a19-c44a-4d35-9390-7c26077aee47.png)
### ModLogs for bans
![image](https://user-images.githubusercontent.com/91988772/185662141-87a9799d-3124-450d-a383-2a53f8830726.png)
### ModLogs for timeouts
![image](https://user-images.githubusercontent.com/91988772/185662407-3587b9dc-9e85-42b7-a682-ce36fa70b950.png)

# Contributing:
> if you want to contribute create a fork of this project and when you are done editing it update the fork and create a pull request.
