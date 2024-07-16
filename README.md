# Deeeep.io Scripts Leak

## PD multiple animal glitch
```js
(game => {
    Object.getOwnPropertyNames(game).map(v=>game[v]).find(v=>typeof(v)=="object"&&v.connect instanceof Function).sendStringPacket(JSON.stringify({ p: 7, e: -1 }));
})(document.getElementById("app")._vnode.appContext.config.globalProperties.$simpleState.states.find(v=>v._storeMeta.id=="game").gameManager)
```
