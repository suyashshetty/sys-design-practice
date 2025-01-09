The list of APIs need to confirm with the in-scope functional requirements
Considering distributed system architechture, state assumption for a microservices architecture 
and define routes for each api endpoint

```
1. Request a short url by posting a long url
/POST /urls -> shortUrl
{
    long-url,
    alias?
    expirationTime?
}

2. Redirection based on short url
/GET {short-url} -> long-url (redirection, 302 - temporary, 301 - permanent)
```