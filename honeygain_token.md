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

# Is this safe?
I'm not going to try and sugarcoat it, but this token is something you should not share with anyone. It is direct access into your honeygain account, if an attacker knows what they are doing. However, I can do my best to assure you that this token is only saved on your files and is only ever used to authenticate with API requests as seen in the api.py file. The entirity of the source code is also open source and if you do not trust the .exe version, you can always use manual installation to make sure you're getting exactly what you see on the files.
