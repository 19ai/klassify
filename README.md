### Klassify

Redis based text classification service with real-time web interface.

### What is Text Classification

Text classification, document classification or document categorization is a problem in library science, information science and computer science. The task is to assign a document to one or more classes or categories.

<https://en.wikipedia.org/wiki/Document_classification>

There are many use cases of document classifiers in real world:

- Spam filters
- Web page classification
- News and and topic categorization
- Sentiment Analysis

### Demo

![klassify](http://i.imgur.com/iG4atNg.gif)

### Installing

    sudo pip install klassify
    

If you don't have an nltk corpus, you'll need to run this:

    python -c 'import nltk; nltk.download("stopwords")' 

You'll also need `redis` installed, check if you have it installed by running this command:

    redis-server

If you get a `command not found`, follow these [instructions](http://redis.io/topics/quickstart)

### Installing on Virtualenv

```
virtualenv foo
source foo/bin/activate
pip install klassify
python -m klassify
```

#### Usage

```
python -m klassify
```

Command line options:

```
  --port                           run on the given port (default 8888)
  --prefix                         prefix that will be used in redis keys
                                   (default klassify)
  --redis-db                       redis database (default 0)
  --redis-host                     redis host (default localhost)
  --redis-port                     redis port (default 6379)
```

