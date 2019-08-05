# User

## Endpoint

```
GET https://www.spielerplus.de/en/user/view?id=<id>
```

**Type:** `HTML`

## Fields

**_Note:_** The selectors target the element containing the text node, not the actual text.

| Field           | Type   | Selector                         |
|:----------------|:-------|:---------------------------------|
| Image           | image  | `.user-icon > div > img`         |
| Name            | string | `.user-name`                     |
| Position        | string | `.user-position`                 |
| Role            | string | `.user-role-item`                |
| Age             | number | `div.col-lg-3:nth-child(1) > h4` |
| Number          | number | `div.col-lg-3:nth-child(2) > h4` |
| Penalties       | string | `div.col-lg-3:nth-child(3) > h4` |
| Shirt size      | ToDo   | `div.col-lg-3:nth-child(4) > h4` |
| Birthday        | date   | `div.col-md-4:nth-child(1) > p`  |
| Address         | string | `div.col-md-4:nth-child(2) > p`  |
| Member since    | date   | `div.col-md-4:nth-child(3) > p`  |
| E-mail address  | ToDo   | `div.col-md-4:nth-child(4) > p`  |
| Phone           | string | `div.col-md-4:nth-child(5) > p`  |
| Passport Number | string | `div.col-md-4:nth-child(6) > p`  |
