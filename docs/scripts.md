# Scripts

---

An overview of how certain scripts should be used.

---

### GameManager

A global manager script that should only handle global tasks, like overall game settings, physics settings, etc.

---

### GlobalReferences

This script will hold references of all manager and handler scripts that are universally required.

---

### LevelManager

LevelManager is responsible for loading the correct level, managing level win and level fail.

---

### SettingsHandler

This script controls the settings panel which holds music and haptic toggles along with the attribution section.

---

### GameState

Defines all possible game states as an enum. Basic states have already been added. You can expand on this and add any major game states to this.

---

### GameEvents

Defines basic events that you can use as required. For example - OnGameStarted, OnGamePaused, OnLevelComplete, OnLevelFailed. You can add any more global events here.

<b><i> Note:</b>  Only add major events that affect the entire game here. Do not add any functionality-specific events here.</i>

---

### CoroutineManager

You can use this script to run any coroutine without being dependant on a monobehaviour object. You can also call coroutines with delay.

It also includes a class called CoroutineWaitDelay which defines constants for delay in seconds. Use these constants whenever you need to define delays.

---

### LevelEndScreenBase

Provides a basic implementation of level complete and level fail screens.

<b><i> Note:</b> For custom implementation of these screens, make sure you extend this class as it provides all basic functionality.</i>

---

### Logger

A custom logger that helps in easier debugging.

You can pass tags to easily search for relevant logs.

---

### FloatingTextManager

This script allows you to easily spawn floating texts that can be used to indicate damage, income, etc.

---

### ButtonAnimator

This script allows us to easily add feedback to buttons. Just assign the event intended for the button and on click the button will now animate and then call the event.

---

### AdsManager

A very basic template that allows for ad integration.

---

### AnalyticsHandler

A very basic template that allows for analytics integration.

---

### SaveManager

Use this script to save persistent data instead of using PlayerPrefs. It also allows saving custom data like dates, images, etc.

---

### StaticInstance, Singleton, PersistentSingleton

These classes allow an easy way to create instances of an object.

<b><i>StaticInstance</i></b> - Creates a static "Instance" variable of the object that can be overwritten. Gets destroyed when scene reloads.

<b><i>Singleton</i></b> - Creates a singleton static "Instance" variable of the object that cannot be overwritten. Gets destroyed when scene reloads.

<b><i>PersistentSingleton</i></b> - Creates a singleton static "Instance" variable of the object that cannot be overwritten. Does not get destroyed when scene reloads.

---

###