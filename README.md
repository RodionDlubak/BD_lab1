# Lab 1. Getting started with basic PostrgeSQL functionality

## Gaming field

Website devoted to selling game accounts.

## Graphical ER model

![ER digram](diagram.png)

| Relation | Attribute | Data type |
|----------|-----------|-----------|
| account | `account_id` - unqiue identifier<br>`login` - account login<br>`password` - account password<br>`created` - date, when account was created<br>| Integer<br>String<br>String<br>Date<br> |
game | `game_id` - unique identifier<br>`game_name` - name of the game<br>`hours_played` - time, spent in game<br>`account` - ID of related account.<br>| Integer<br>String<br>Integer<br>Integer<br> |
item |`item_id` - unique identifier<br>`item_name` - name of the item<br>`price` - real cost of item (in USD)<br>`game` - ID of related game<br>| Integer<br>String<br>Numeric<br>Integer<br> |
