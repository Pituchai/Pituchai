update comment, delete comment 
## Comment on the review   ##
write comments on the review.

## URL ##
`POST /type`

## REQUEST BODY ##
REQUEST BODY


| Parameter	    |      Type     | Description |
| ------------- | ------------- |-------------| 
| comment_ID    | int           | comment's id|


EXAMPLE 
```

{
 comment_ID: "c3d321d32s23"

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
 commentText: "Hello your reveiw  is good,it's help me a lot"
 commentDate: "10-6-22"
 amountLike : 23 

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


