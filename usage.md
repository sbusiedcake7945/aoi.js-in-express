# usage

how to use it
```js
app.get("/guild/prefix/:guildID", (req, res) => {
const { guildID } = req.params;

const guild = client.guilds.cache.get(guildID);

const prefix = await $aoiEval(`$getGuildVar[prefix;${guildId}]`);
});
res.json(guildID, prefix)
```
you can use it like this but you need aoi.js and express.js

[![express docs](./express.svg)](https://expressjs.com)

[![aoi.js docs](./aoi.js.svg)](https://aoi.js.org/)