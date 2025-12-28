<style>
  body {
    bacground-color: black;
    color: white;
  }
</style>
# first step

add
```js
const Interpreter = require("aoi.js/src/core/interpreter.js");


function $aoiEval(codeStr) {
    try {
        const messageContext = {
        channel: { send: async () => {} },
        author: client.users.cache.get(userId) || { id: userId },
        guild: guild || null,
        member: member || null,
        message: {}
        };

const result = await Interpreter(
    client,
    messageContext,
    [],
    { code: codeStr },
    client.db,
    true,
    undefined,
    {},
    undefined,
    false,
    false,
    false,
    false
    );

    return result?.code ?? null;
    } catch (err) {
        console.error("Interpreter error:", err);
        return null;
        }
        }
```
# examples


[![examples](./button2.svg)](./usage)

