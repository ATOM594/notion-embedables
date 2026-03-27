# notion-embedables

## Timer

<img src="timer/images/timer.png" alt="timer.png" width="30%">

A customizable countdown timer that can be embedded in Notion or can be used in any browser of your choice.

### Features

- **Editable Timer**: Click on the timer to edit the time directly
- **Flexible Input Formats**:
  - Single number: `10` (interpreted as minutes)
  - Minutes:Seconds: `10:30` (10 minutes 30 seconds)
  - Hours:Minutes:Seconds: `1:30:45` (1 hour 30 minutes 45 seconds)
  - Days:Hours:Minutes:Seconds: `2:01:30:45` (2 days 1 hour 30 minutes 45 seconds)
- Press **Enter** to start the timer
- Press **Escape** or click outside the timer to cancel editing

### Usage

Base URL: `https://atom594.github.io/notion-embedables/timer`

**Default:** 10 minutes (if no parameters are set)

### Parameters

Set the initial timer duration using URL parameters:

- **Minutes**: `m`, `min`, `mins`, or `minutes`
- **Seconds**: `s`, `sec`, `secs`, or `seconds`
- **Hours**: `h`, `hour`, or `hours`
- **Days**: `d`, `day`, or `days`

### Examples

**10 minute timer:**
```
https://atom594.github.io/notion-embedables/timer?m=10
```

**5 minute 30 second timer:**
```
https://atom594.github.io/notion-embedables/timer?m=5&s=30
```

**1 hour timer:**
```
https://atom594.github.io/notion-embedables/timer?h=1
```

**2 hours 15 minutes:**
```
https://atom594.github.io/notion-embedables/timer?h=2&m=15
```

**1 day countdown:**
```
https://atom594.github.io/notion-embedables/timer?d=1
```

### Embedding in Notion

1. Copy the timer URL with your desired parameters
2. In Notion, type `/embed`
3. Paste the URL
4. The timer will appear as an interactive embed

**Note:** The timer automatically adapts to your system's dark/light mode setting. Notion prevents embedded iframes from accessing Notion's own theme settings, so the timer cannot match Notion's theme directly.
