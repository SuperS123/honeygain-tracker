# How do you get your token?

It's very simple, here are the 2 easiest methods

1. Automatic (Simple but requires trust)
--------------------------------------------------------------------------------
Just run this code after opening Dev Tools (right click anywhere and click Inspect Element) and opening the "Console" tab
```javascript
navigator.clipboard.writeText(localStorage.getItem("JWT"))
console.log(localStorage.getItem("JWT"))
console.log("The above message is your token, it was also copied to your clipboard")
```

2. Manual (Longer, but you can see what you're doing)
--------------------------------------------------------------------------------
* Go to [the honeygain dashboard](https://dashboard.honeygain.com/)
* Open Dev Tools (right click anywhere and click Inspect Element)
* Click Application (if you don't see it, click the 2 arrows)
* Click the arrow next to local storage
* Click dashboard.honeygain.com
* Copy the value next to JWT

You successfully got your token.
