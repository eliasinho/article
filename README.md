## Installation

To install Postman, just go to [this link](https://www.getpostman.com/apps) and download the right version for the OS you use.

## How to do a simple GET ?

Now, you should see the following screen :

![First screen](WhatsApp Image 2018-02-02 at 14.14.14.jpeg)

Click the **Request** button at the top-left of the modal, and you'll get on the **Save Request** screen.

Give it a name, select a collection and save it.

![Request screen](save-my-request.png)

From there, you'll be able to send a request. For exemple, you can hit the `HTTPCat` API. Just enter the `https://http.cat/[status_code]` URL in the dedicated tab, with the status code of your choice. Press **Send** and you'll see the response just below.

![Get cat image](get-request.png)

## A first POST with a JSON body

To do a `POST` request, we are going to hit the `https://jsonplaceholder.typicode.com/` URL, on the `post` route.

So from the same screen, select `POST` instead of `GET`, and enter the URL in the dedicated tab.

![First POST](post-try.png)

The API we're hitting enables us to send any JSON body, and sends it back in the response, adding it an `id`. Let's then send a random object.

Go in the **Body** tab, check the **raw** radio button, and make sure that you selected **JSON (application/json)** on the dropdown on the right.

Now let's right our JSON object. There are a couple things we need to be careful of when we right a JSON object, especially when you are used to do JavaScript.

### Use quotes for the object keys

:no_entry_sign:

```
{
	key: "string"
}
```

:white_check_mark:

```
{
	"key": "string"
}
```

### Use double quotes

:no_entry_sign:

```
{
	'key': "string"
}
```

:white_check_mark:

```
{
	"key": "string"
}
```



![Object](post-object.png)


- mettre des double quotes et pas des singles quotes
- body d'un POST en 'raw'
- Si c'est un JSON penser à spécifier 'application/json'
- pas de virgule après le dernier élément de ton json
- false et true sont en minuscule

