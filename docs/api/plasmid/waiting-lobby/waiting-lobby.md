# Waiting Lobby
The Waiting Lobby is a global implementation used by a lot of Plasmid Minigames. It affects things like block breaking, player damage, provides a ready-up system and handles private games for you automatically. The only methods it exposes are to add the waiting lobby and to change the sidebar's contents.  
![Image showing what the waiting lobby looks like](../../../assets/images/api/waiting-lobby.png)  

### GameWaitingLobby.addTo(GameActivity, WaitingLobbyConfig)

---
This is a static method that applies this waiting lobby implementation to the [GameActivity](../game-activity.md), given the [WaitingLobbyConfig](waiting-lobby-config.md). You are not meant to initialize the WaitingLobby using the constructor, as it is private.
### setSidebarTitle(Component)  

---
Sets the Title of the Waiting Lobby Sidebar.

### setSidebarLines(List\<Component>)  

---
Sets the content of the sidebar to the list of Components provided.
