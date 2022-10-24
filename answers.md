## Question 1:
Hello,

I'm new to search engines, and there are a lot of concepts I'm not educated on. To make my onboarding smoother, it'd help if you could provide me with some definitions of the following concepts:
- Records
- Indexing

I'm also struggling with understanding what types of metrics would be useful to include in the "Custom Ranking." 

Cheers,
George


## Answer:

Hi George,

Thank you for reaching out. 

Records:

A record is a single entry in an index that you want users to be able to search for.  For example, if you run an ecommerce store that sells t-shirts, each t-shirt that you want users to find and purchase on your website will represent one record.

Records are made up of structured key-value pairs. For t-shirts, this could like below:

```
{
  "name": "Black t-shirt",
  "brand": "Polo",
  "color": "Red",
  "price": 70
}

```

Indexing:

Indexing refers to the process of adding, updating or deleting records from your Algolia index (you can think of your index as your Algolia database). 

For example, if you have added a new product to your catalogue and you want users to search for that product, you can add it to your Algolia index - this process is an indexing operation. Likewise, if you delete the same product from your index, this is also an indexing operation.



## Question 2:
Hello,

Sorry to give you the kind of feedback that I know you do not want to hear, but I really hate the new dashboard design. Clearing and deleting indexes are now several clicks away. I am needing to use these features while iterating, so this is inconvenient.

Regards,
Matt


## Answer:


## Question 3:
Hi,

I'm looking to integrate Algolia in my website. Will this be a lot of development work for me? What's the high level process look like?

Regards,
Leo

## Answer:

Hi Leo,

Good to hear you are looking to integrate Algolia onto your website.

The high levesl process:

1. Organising and indexing your data



2. Configuring search relevancy settings
3. UI and frontend integration

