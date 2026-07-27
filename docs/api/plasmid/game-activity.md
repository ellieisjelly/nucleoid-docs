# Game Activity
Every [GameSpace](game-space.md) in Plasmid is controlled by a GameActivity that handles the event loop and all game logic contained to this game. For a GameActivity to be considered active, it must be applied to a [GameSpace](game-space.md). There can only be one active GameActivity at once, however it can be easily changed by using the [setActivity](game-space.md#setActivity) method of [GameSpaces](game-space.md).  
### getGameSpace()

---
Returns the current [GameSpace](game-space.md) attached to this GameActivity.

### setRule([GameRuleType](game-rule-type.md), [EventResult](event-result.md))

---
Sets whether a given [GameRuleType](game-rule-type.md) can be executed based on the [EventResult](event-result.md).

### allowRule([GameRuleType](game-rule-type.md))

---
Equivalent to setRule([GameRuleType](game-rule-type.md), [EventResult.ALLOW](event-result.md#allow));

### denyRule([GameRuleType](game-rule-type.md))

---
Equivalent to setRule([GameRuleType](game-rule-type.md), [EventResult.DENY](event-result.md#deny));

### listen(StimulusEvent\<T>, T listener)

---
Registers a listener for the [StimulusEvent](../stimuli/stimulus-event.md) that gets triggered in this Activity.

### addResource(AutoCloseable)

---
Adds a resource that gets closed automatically when the GameActivity is deleted.

