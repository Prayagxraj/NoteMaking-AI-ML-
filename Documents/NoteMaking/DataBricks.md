We will try to learn dataBricks in a simple way 

->Model = Brain 
-> Registry = Storage
->Endpoint= Door

What is a Model ?
def Model(x) :
      return "Hello" + x


This is a Model 

input -> "Prayag"
output -> "Hello Prayag"

In simple Terms 
Model = function (input -> output)



## Why cant we just Keep a Notebook ?

Your Notebook 
Runs-> works
Stops->Everything gone 

Real world Problem : If your manager says Give me this model tomorrow. You say Wait let me run my notebook ? hahaha



Solution ? You save the model 

Notebook model -> Saved file (Artifacts)

## What is a Model registry ?

Lets imagine you save many models like 
model1_v1
model1_v2
model1_v3

there is some problem in tis that we dont know which one to use ? which one is correct ?

So the solution is  ##Model Registry 

You can say Model registry = Google Drive for Models

![img](/Users/prayagraj/Downloads)


## What is End-Point ?
 
 You have built a model How will someone use it ??

##Wrong way = They open Notebook
##Correct way = We create Door(API) 

That Door is Serving Endpoint


##What we do with curl .....

It means we knocked the door

and the response is ["Hello world Prayag!!"]


Door opened --> Model ran --> You got answer 




Simple Story ->

1 You created Model(Brain)
2 You saved Model(ML Flow)
3 You organised Registry
4 You build Endpoint(Door)
5 Used Curl (You knocked)
6 Got response



##Model Registry = A place where your saved models are organised and versioned

Without it :- 1) Hard to remember 2)No versions 3) Cannot manage and deploy properly

with it :-  1) Clean Name  2)Version Contol 3) Easy deployment and Production ready

##End point = Rest API service running your model


1. Receives request (JSON)
2. Checks schema (input format)
3. Sends to model
4. Gets output
5. Returns response



Client (curl)
   ↓
HTTP Request
   ↓
Endpoint Server
   ↓
Schema Validation
   ↓
Load Model (from Registry)
   ↓
Call predict()
   ↓
Return JSON response

