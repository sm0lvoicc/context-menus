# context-menus
once baby jesus said, He who shall be last shall be sideways and smiling  
idk why i said this but okay,  
context menus, so what are they?
![command showcase](https://cdn.discordapp.com/attachments/767941058138996766/870618022207971368/image0.gif)
okay so this is how they work, now, time to see, eh, the types
## User ones
so these are
type: 2
to make them you do 
```js
applications(application.id).commands.post({
  type: 2,
  name: "rickroll"
});
```
and these commands will be shown as like
![image](https://user-images.githubusercontent.com/72088954/128939531-db3c3f65-f051-4f6b-bac9-fa223358f341.png)
## message ones
type: 3
to make them you do 
```js
applications(application.id).commands.post({
  type: 3,
  name: "rickroll"
});
```
![image](https://user-images.githubusercontent.com/72088954/128939840-9595f475-44ab-4133-b06a-d0e5601000a2.png)

## recieved interaction
everything is the same except the interaction.data has `target_id` and `resolved`
for message the resolved field will have a json of message object with message id as the parent, the message if will be the same as the `target_id` in interaction.data and same goes visa versa,  
thank you,  
bye  
### DISCORD STUFF
[Docs for user commands](https://discord.com/developers/docs/interactions/application-commands#user-commands)  
[Docs for message commands](https://discord.com/developers/docs/interactions/application-commands#message-commands)
