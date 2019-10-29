# Routing Notes

[client] ==> a request ==> [api] ==> response [client]

Interface for a web api? ==>

- URI (uniform resource identifier)
- URL (universal resource loader)
- Endpoint (very related to uri)
- HTTP === network protocall, a set of rules for communication

REST(ish)

- everything is a 'resource'
- single URI per resource i.e. 'http:/web23.com/channels', 'http:/web23.com/channels/users', 'http:/web23.com/channels/threads'
- use HTTP methods to perform operations on resources

| non REST         | REST             |
| :--------------- | :--------------- |
| /listAllChannels | GET /channels    |
| /createChannel   | POST /channels   |
| /updateChannel   | PUT /channels    |
| /deleteChannel   | DELETE /channels |
| /findChannel/:Id | GET /channel/:id |

What is an Express Router? Why is it useful?

An express router can have route/request handlers and middleware

## Query String

https://www.google.com/search
?
q = express.js
&
oq = express.js
&
aqs = chrome.0.0l5j69i61.3353j0j7
&
sourceid = chrome
&
ie = UTF-8

```js
req.query = {
    q: 'express.js',
    oq: 'express.js',
    ...
    ie: 'UTF-8'
}
```
