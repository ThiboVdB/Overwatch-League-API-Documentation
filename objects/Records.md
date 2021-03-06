<img src="https://bnetcmsus-a.akamaihd.net/cms/page_media/kz/KZFG2DZCYMAJ1551917378814.jpg">

# Records
Records maintain information about a Team's statistics. 

## Records Data Dictionary
| Attribute           | Type  | Description |
|:--------------------|:------|:------------|
|`matchWin`|Int64|The number of wins scored by a Competitor.|
|`matchLoss`|Int64|The number of losses scored by a Competitor.|
|`matchDraw`|Int64|The number of tie games scored by a Competitor.|
|`matchBye`|Int64|The number of times a Competitor advances to the next round if the Competitor does not have an opponent. This allows the League to run smoothly.|
|`gameWin`|Int64|The number of total game wins scored by a Competitor.|
|`gameLoss`|Int64|The number of total game losses scored by a Competitor.|
|`gameTies`|Int64|The number of total tie games scored by a Competitor.|
|`gamePointsFor`|Int64|The number of total game points earned by the Competitor|
|`gamePointsAgainst`|Int64|The number of total tie games scored by a Competitor's opponents.|
|`comparisons`|Array of Comparison Objects|A list of comparison methods and values used to rank players. Each Comparison object has a `key`: a comparison method, and a `value`: the comparison differential.| 

## Sample Records JSON
```json
"records": {
    "matchWin": 1,
    "matchLoss": 1,
    "matchDraw": 0,
    "matchBye": 0,
    "gameWin": 3,
    "gameLoss": 5,
    "gameTie": 0,
    "gamePointsFor": 0,
    "gamePointsAgainst": 0,
    "comparisons": [
        {
            "key": "MATCH_DIFFERENTIAL",
            "value": 0
        },
        {
            "key": "MATCH_GAME_DIFFERENTIAL",
            "value": -2
        },
        {
            "key": "GAME_HEAD_TO_HEAD_DIFFERENTIAL",
            "value": null
        },
        {
            "key": "MATCH_HEAD_TO_HEAD_DIFFERENTIAL",
            "value": null
        },
        {
            "key": "ADVANTAGE",
            "value": 0
        }
    ]
}
```