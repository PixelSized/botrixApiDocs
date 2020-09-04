Documentation:

IMPORTANT: Need an authentication token? Botrix.tk/developers


------------------------------------------------------

## GET /api/get/bot/:id

Authentication: Requires Bearer Token

Get's a bot's stats from id 

See [bot object] for more info on this endpoint

------------------------------------------------------

## GET /api/get/user/:id

Authentication: Requires Bearer Token

Get's user stats and bot's listed on website

See [user object] and [bot object] for more info on this endpoint

------------------------------------------------------

## GET /api/protected/users/voted/:id

Authentication: Requires Bearer Token

Get's if the user has voted for your listed bot's


---------------------------------------------------------


User Object

| Field | Data type | Description  |
|-------|-----------|--------------|
| id | string | user id from discord|
| username | string | their discord username |
| bot | bool | gets if they are a bot |
| discriminator | string | get's their DiscordTag |
| avatar | string | Get's their avatar url | 
| flags | int | get's user flags |


Bot Object


| Field   | Data type | Description  |
|-------|-----------|--------------|
| botTags | array | tags used in bot |
| usersVoted | string | users voted |
| state | string | verifacation state |
| owners | array | owners id |
| nsfw | bool | is nsfw | 
| username | string | bot's username |
| botId       | string | bot's id |
| logo        | string | avatar url for bot |
| invite      | string | bot's invite |
| description | string | short description for bot |
| long | string | long description for bot (markdown) |
| prefix | string | bot's prefix |
| addedAt | string | date added |
| support | string | support server invite |
| website | string | bot's webiste |


