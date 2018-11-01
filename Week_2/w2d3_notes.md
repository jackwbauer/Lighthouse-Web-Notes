# Week 2 Day 3 Notes

Route -
1. VERB
2. path to resource

GET /login
POST /login
PUT /login

POST - creating new resource on the server
PATCH - changing resource on the server

HTTP Status code

## URL vs URI

URL - Uniform Resource Location
URI - Uniform Resource Indentifier

All URLs are URIs. Not all URIs are URLs.

BREAD:
Browse - GET /nouns
Read - GET /nouns/:id
Edit - GET /nouns/:id/edit | PUT or PATCH nouns/:id
Add - POST /nouns
Delete - DELETE /nouns/:id

## REST

Representational State Transfer - the path that you are going to should represent the data being transfered4

/nouns
/nouns/verb
/nouns/:id
/nouns/:id/verb