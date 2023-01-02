# FlaskGist

Flask GitHub API app to get any user's Gist contributions 

## Search the user
![1](https://user-images.githubusercontent.com/81184255/210281653-d4b1119b-14a4-4954-9d70-da858cab09a9.jpg)

## Each gist will have the last three fork owners displayed
![2](https://user-images.githubusercontent.com/81184255/210282348-7b535d4e-8abe-4639-b68e-9e170333f8f3.jpg)

## When clicked, the gist will show the content along with a GitHub-like language tag
![3](https://user-images.githubusercontent.com/81184255/210282386-ad0c5b12-88d2-40d5-8474-077635b11a9d.jpg)

> **Warning**
> Sometimes the GitHub APi will reach its limit (60 request/h/ip).

To check your status, use this:

```bash
> curl -I https://api.github.com/users/YourUserName
```

> **Note**
> This will give you the Unix time for your reset limit like this:

```
X-RateLimit-Reset: 1672698829
```

You can then use an epoch time stamp converter like [this one](https://www.unixtimestamp.com/) to get the relative time.


