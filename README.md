update comment, delete comment 
## Comment on the review   ##
show user who write comments on the review.

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

| Parameter	    |      Type     | Description |
| ------------- | ------------- |-------------| 
| commentText   | String        | comment text|
| commentDate   | Datetime      | time that comment|
| amountLike    | Int           | number of user like comment|

EXAMPLE

```

{
 commentText: "Hello your reveiw  is good,it's help me a lot"
 commentDate: "10-6-22"
 amountLike : 23 

}

```
 
#### fail 
`400 /fail`

