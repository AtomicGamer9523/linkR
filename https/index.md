# Endpoints

### Please specify your <u>TOKEN</u> as a value of the '<u>linkr-token</u>' key in headers

## **`GET`** [`/`](https://www.docs.linkrbot.com)

Redirects to [docs](https://www.docs.linkrbot.com).

<br>

## **`GET`** [`/test`](https://www.api.linkrbot.com/test)

Used for testing connection.

<br>

## **`GET`** [`/users/`{<u>LINKR-USER-ID</u>}`/links`](https://www.api.linkrbot.com/users/LINKR-USER-ID/links)

Returns all public links of the user.

<br>

## **`GET`** [`/users/`{<u>LINKR-USER-ID</u>}`/links/`{<u>LINK-TYPE</u>}](https://www.api.linkrbot.com/users/LINKR-USER-ID/links/LINK-TYPE)

Returns the users link you specified, only public ones.

<br>

## **`GET`** [`/finduser/`{<u>SERVICE</u>}`/`{<u>UUID</u>}](https://www.api.linkrbot.com/users/LINKR-USER-ID/links/LINK-TYPE)

Trys to find a a matching result. returns allways the first result. `404` if doesn't find anything

<br>