# Event

There are four types of events: event, game, tournament and training. They mostly share the same fields, additional ones are listed below.

## Endpoints

```
GET https://www.spielerplus.de/en/event/view?id=<id>
```

```
GET https://www.spielerplus.de/en/game/view?id=<id>
```

```
GET https://www.spielerplus.de/en/tournament/view?id=<id>
```

```
GET https://www.spielerplus.de/en/training/view?id=<id>
```

**Type:** `HTML`

## Fields

**_Note:_** The selectors target the element containing the text node, not the actual text.

| Field       | Type         | Selector                                                                                            |
|:------------|:-------------|:----------------------------------------------------------------------------------------------------|
| Headline    | string       | `.main-header > div:nth-child(1) > div:nth-child(1)`                                                |
| Subline     | string       | `.main-header > div:nth-child(2)`                                                                   |
| Confirmed   | number       | `div.participation-widget:nth-child(1) > div:nth-child(1) > button:nth-child(1) > div:nth-child(2)` |
| Unsure      | number       | `div.participation-widget:nth-child(1) > div:nth-child(1) > button:nth-child(2) > div:nth-child(2)` |
| Declined    | number       | `div.participation-widget:nth-child(1) > div:nth-child(1) > button:nth-child(3) > div:nth-child(2)` |
| Meet        | string       | `div.col-xs-4:nth-child(1) > div:nth-child(1) > div:nth-child(2)`                                   |
| Begin       | string       | `div.col-xs-4:nth-child(2) > div:nth-child(1) > div:nth-child(2)`                                   |
| End         | string       | `div.col-xs-4:nth-child(3) > div:nth-child(1) > div:nth-child(2)`                                   |
| End         | string       | `div.col-xs-4:nth-child(3) > div:nth-child(1) > div:nth-child(2)`                                   |
| Description | string       | `.event-description > .text-center`                                                                 |
| Address     | string       | `.info-area-content > small:nth-child(2)`                                                           |
| Tasks       | List\<Task\> | ToDo                                                                                                |
| Carpool     | List\<Car\>  | ToDo                                                                                                |
| Lineup      | ToDo         | ToDo                                                                                                |

### Taks

ToDo

### Car

ToDo

### Tournament only

| Field        | Type   | Selector                                                          |
|:-------------|:-------|:------------------------------------------------------------------|
| Bring along  | string | `div.list-item:nth-child(2) > div:nth-child(2)`                   |
| Catering     | string | `div.list-item:nth-child(3) > div:nth-child(2)`                   |
| Game         | string | `div.list-item:nth-child(4) > div:nth-child(2)`                   |
| Opponents    | string | `div.list-content-label-sublabel:nth-child(1) > div:nth-child(2)` |
