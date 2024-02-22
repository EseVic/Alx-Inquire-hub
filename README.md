
# ALX - Inquire Hub

InquireHub is an innovative AI-Powered web application that engages in intuitive and accurate conversations with users. InquireHub is designed to understand user queries deeply, allowing it to provide intuitive responses that address specific needs. 


## Acknowledgements

 - [OpenAI](https://openai.com)
 - [ALX Africa ](https://alx.com)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## API Reference

#### Get a user's conversations from db

```http
  GET /api/conversations
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Not Required**. |
| `admin_role` | `boolean` | **Required**. |


#### Get a user's articles from db 

```http
  GET /api/articles
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Not Required**. |
| `admin_role` | `boolean` | **Required**. |

#### Get a user's generated code snippets from db 

```http
  GET /api/code
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Not Required**. |
| `admin_role` | `boolean` | **Required**. |

#### Get all registered users

```http
  GET /api/users
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Not Required**. |
| `admin_role` | `boolean` | **Required**. |

#### Get a registered individual account

```http
  GET /api/users/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of user to fetch |

#### Authenticate and start a user session 

```http
  POST /api/login
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Not Required**. |
| `login_token` | `string` | **Required**. |

#### Make a conversation request via openAI 

```http
  POST /api/conversations
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. OpenAI API key |
| `login_token` | `string` | **Required**. |

#### Make an article generation request via openAI 

```http
  POST /api/articles
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. OpenAI API key |
| `login_token` | `string` | **Required**. |

#### Make code snippets generation request via openAI 

```http
  POST /api/code
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. OpenAI API key |
| `login_token` | `string` | **Required**. |

#### Pro membership subscriptions 

```http
  POST /api/paystack/pay
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Paystack API key |
| `login_token` | `string` | **Required**. |



## Authors

- [Victoria Iria](https://github.com/EseVic)
- [Israel Oyetunji](https://github.com/x9x96)
- [Peter Odo](https://github.com/Odo-Peter)


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file. These keys are obtained from the official websites of openai, paystack and mongo atlas, treat these keys as passwords and keep them safe.

`OPENAI_API_KEY`

`PAYSTACK_SECRET_KEY`

`MONGODB_URI`


## Features

- Human like conversation
- Succint and detailed article generation
- Accurate code generation snippet
- Appealing user inteface
- Ease of use
- Cross platform
- Responsive layout


## FAQ

#### Do I have to subscribe before using the platform?

No, every newly registered user has a free trial tier, this user can query the AI for accurate answers. This free tier comes with only five queries per user.

#### How soon does my limit reflects when I subscribe?

As soon as the subscription is done, it immediately reflects, thanks to the optimization from the developers. The sidebar of the web app is automatically updated to your subscribed plan.


## Tech Stack

**Client:** React, Redux, TailwindCSS

**Server:** Node, Express, Mongoose

**API:** OpenAI, Paystack


## Run Locally

Clone the project

```bash
  git clone https://github.com/EseVic/Alx-Inquire-hub/
```

Go to the project directory

```bash
  cd Alx-Inquire-hub
```

Install dependencies

```bash
  npm install
```


Create a .env file and add env variables

```bash
  touch .env
```

Start the server

```bash
  npm run dev
```


## Screenshots
![Landing Page](https://github.com/EseVic/Alx-Inquire-hub/assets/108824188/74d6777b-13ed-4e60-b0ed-98f9c4784d2b)

![Sign In](https://github.com/EseVic/Alx-Inquire-hub/assets/108824188/a18f0352-b2bc-4f2b-a6a1-54e70d1a8082)

![Home](https://github.com/EseVic/Alx-Inquire-hub/assets/108824188/590f058b-4f83-4df6-936a-4e379f464e07)




