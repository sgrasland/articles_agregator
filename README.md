# Website articles links fetcher

Node.js app to send website articles links to a receiver (Notion, E-mail, ...)

Micro-services architecture composed with :
  - A service that reads websites and fetch the list of new articles to read : **WebsiteReader**
  - A service that transmit new articles links to a receiver : **ArticlesTransmitter**

## WebsiteReader

This service starts one background task for each website declared in config :

![WebsiteReaderService](https://user-images.githubusercontent.com/47080041/154859398-8a6d6d5e-7ccb-4992-be40-068c29d4ec9a.PNG)

Implementation :

![WebsiteReaderService_Implementation](https://user-images.githubusercontent.com/47080041/154859423-579e9207-c7ab-4e8c-96da-dd31f8a17547.PNG)
