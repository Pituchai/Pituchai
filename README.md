update comment, delete comment 
## Comment on the review   ##
write comments on the review.

## URL ##
`POST /type`

## REQUEST BODY ##
REQUEST BODY

| Parameter	    |      Type     | Description |
| ------------- | ------------- |-------------|
| Review_ID     | int       | review's id|
| Comment_ID    | int       | comment's id  |
| User_ID       | String        | user' id who write on review   |
| commentText   | String     | comment on reveiw |
| commentDate   | Datetime      | date comment|

EXAMPLE 
```

{
 review_ID : "d784129589"
 comment_ID: "c3d321d32s23"
 user_ID : "j312513d12" 
 commentText:"This is good reveiw, it's help me a lot"
 commentDate:"10-6-22"

}

```
#### success

RESPONSE

| Parameter	    |      Type     | Description |
| ------------- | ------------- |-------------|
| Review_ID     | int       | review's id|
| Comment_ID    | int       | comment's id  |
| User_ID       | String        | user' id write on review   |
| commentText   | String     | comment on reveiw |
| commentDate   | Datetime      | date comment|
| amountLike    | int           | number of user like comment|

EXAMPLE

```

{
 review_ID : "d784129589",
 comment_ID: "c3d321d32s23",
 user_ID : "j312513d12" ,
 commentText:"This is good reveiw, it's help me a lot",
 commentDate:"10-6-22",
 amountlike : "20"

}

```
 
#### fail 
`400 ` fail
***

## Delete comment on the review   ##
delete comment by comment_ID

## URL ##

`DELETE /:id`

## REQUEST BODY ##
REQUEST BODY


| Parameter	    |      Type     | Description |
| ------------- | ------------- |-------------| 
| comment_ID    | int           | comment's id|

EXAMPLE

```

{
 comment_ID: "c3d321d32s23",
}

```
#### success
`200 ` ok
#### fail
`200 ` bad request
***




