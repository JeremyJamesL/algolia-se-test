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

Thank you for reaching out. I have given definitions of each of the concepts below for you:

### Records:

A record is a single entry in an index that you want users to be able to search for.  For example, if you run an ecommerce store that sells t-shirts, each t-shirt that you want users to find and purchase on your website will represent one record.

Records are made up of structured key-value pairs. For t-shirts, one records could look like the following:

```
{
  "name": "Black t-shirt",
  "brand": "Polo",
  "color": "Red",
  "price": 70
}

```

### Indexing:

Indexing refers to the process of adding, updating or deleting records from your Algolia index. 

For example, if you have added a new product to your catalogue and you want users to search for that product, you can add it to your Algolia index - this process is an indexing operation. Likewise, if you delete the same product from your index, this is also an indexing operation.

### Custom ranking metrics

You can think of custom ranking metrics as business specific metrics that you want to be used to reorder results to better align with your business goals. 

For example, if you are an ecommerce company that needs better visibility for on sale items and your records have an on sale attribute, for example ```"onSale": true```, then adding ```onSale``` as a custom ranking attribute will mean that for records with textual relevance equality, those that are on sale will be more highly ranked than those that are not.


## Question 2:
Hello,

Sorry to give you the kind of feedback that I know you do not want to hear, but I really hate the new dashboard design. Clearing and deleting indexes are now several clicks away. I am needing to use these features while iterating, so this is inconvenient.

Regards,
Matt


## Answer:

Hi Matt,

Sorry to hear that you aren't enjoying the new design. I will be sure to pass your feedback onto the product team.

That being said, for every operation you are able to perform in the dashboard, we have an API method. For example, to delete an index we have the delete method: https://www.algolia.com/doc/api-reference/api-methods/delete-index/, likewise for clear indices: https://www.algolia.com/doc/api-reference/api-methods/delete-index/. 

You may find it more convenient to build these methods into your workflow while iterating.

## Question 3:
Hi,

I'm looking to integrate Algolia in my website. Will this be a lot of development work for me? What's the high level process look like?

Regards,
Leo

## Answer:

Hi Leo,

Good to hear you are looking to integrate Algolia onto your website. We have gone to great efforts to make integrating search as simple and quick as possible for developers, and to reduce the amount of development work required.

Here is a high level overview, which will give you a good idea of the amount of work involved:

1. Organising and indexing your data

This involves getting your search data into the Algolia index. First you must create an index, then add your records to the index using our indexing methods: https://www.algolia.com/doc/api-client/methods/indexing/. If you have one product file (note that we expect JSON records) then this is usually just one or two lines of code. 

You also have the option of manually uploading your JSON file via the dashboard. This guide should help: https://www.algolia.com/doc/guides/sending-and-managing-data/send-and-update-your-data/how-to/importing-from-the-dashboard/ 


2. Configuring search relevancy settings

This next step involves configuring the search relevancy settings within your Algolia dashboard. Configuring search relevancy ensures that your users will get the best search results in all situations. A full guide on configuring search relevancy can be found here: https://www.algolia.com/doc/guides/managing-results/relevance-overview/.

3. UI and frontend integration

Now we have the search data in the index, and relevancy configured, all that's left to do is build a search UI for your users to interact with. We have a very convenient open source UI-library called InstantSearch, which lets you easily build a search interface by handling all search componentry via front-end widgets. 

You can be up and running in a matter of minutes. Please read more here: https://www.algolia.com/doc/guides/building-search-ui/what-is-instantsearch/js/.

If you would like more control over your frontend components you can create custom InstantSearch widgets: https://www.algolia.com/doc/guides/building-search-ui/what-is-instantsearch/js/. Alternatively you can skip InstantSearch altogether and use one of our API clients for greater UI control: https://www.algolia.com/doc/api-client/getting-started/install/javascript/?client=javascript.

Hope that helps!

