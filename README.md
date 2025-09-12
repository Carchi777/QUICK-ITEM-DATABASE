# introduction
I made this to fix the **main issue** of Minecraft's script api: **you cant save ItemStacks in a dynamic property**, and if you try to stringify its properties you will still loose some of them that are unreacheable with scripts. **This database fixes this problem using structures saving perfect item clones, making it easy, reliable and fast**....

# How does it work?

- This database uses **structures** to save items, it uses an **entity with 255 slots** instead of just dropped items to minimize the lag of the loaded entities, this makes the database have **255 items per key**.

# Features
- **Keys are unlimited**, they re handled by the QIDB class where you put namespace, **cache** size, saves per tick(may change) and developer debug **logs**.

- Cache memory requires a lot of **ram** so i added an option to **limit the cached key amount**.

- Background Saving is made with a **runinterval** that saves an amount of **keys per tick**, to not overload or freeze the game, in **V3.8.4** it uses **RunJob** that may cause** lag** in some devices, insted **V3.8.3** uses a **runinterval** making it more **constant and controllable**.

- Developer debug shows the **logs** in the **console** like how much** time** a function has taken.

# What you can do with this?
```diff
+You can use this script for your addon or server freely and edit it as you want to fit your addon or server. The only requirement is including credits.
+You can create custom versions of this forking the repository.

-You cannot sell this script or redistribute using ad-links.
-You cannot redistribute this claiming this as yours.
```

# Contributes
Thanks to Drag0nD that helped me a lot in the creation of the database and gave me the structure method sending me his infinite chest addon.
https://youtu.be/Trljwe6zay8?si=Yf1gC0ZsvOyAXXEP
