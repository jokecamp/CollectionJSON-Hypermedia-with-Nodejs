This is an implementation of the following tutorial on Hypermedia APIs using the Collection+JSON hypermedia type and Node.js

http://amundsen.com/media-types/tutorials/collection/tutorial-01.html

### To Run
run the following from your root project directory:

```node server.js```

then vist http://localhost:1337


### Example Collection+JSON Hypermedia Response
```json
{
    "collection": {
        "version": "1.0",
        "href": "http://localhost:1337/",
        "links": [{
            "rel": "home",
            "href": "http://localhost:1337"
        }],
        "items": [{
            "href": "http://localhost:1337/mildred",
            "data": [{
                "name": "name",
                "value": "mildred",
                "prompt": "name"
            }, {
                "name": "email",
                "value": "mildred@example.com",
                "prompt": "email"
            }],
            "links": [{
                "rel": "alternate",
                "href": "http://example.com/blogs/mildred",
                "prompt": "blog"
            }]
        }, {
            "href": "http://localhost:1337/mike",
            "data": [{
                "name": "name",
                "value": "mike",
                "prompt": "name"
            }, {
                "name": "email",
                "value": "mike@example.com",
                "prompt": "email"
            }],
            "links": [{
                "rel": "alternate",
                "href": "http://example.com/blogs/mike",
                "prompt": "blog"
            }]
        }, {
            "href": "http://localhost:1337/mary",
            "data": [{
                "name": "name",
                "value": "mary",
                "prompt": "name"
            }, {
                "name": "email",
                "value": "mary@example.com",
                "prompt": "email"
            }],
            "links": [{
                "rel": "alternate",
                "href": "http://example.com/blogs/mary",
                "prompt": "blog"
            }]
        }, {
            "href": "http://localhost:1337/mark",
            "data": [{
                "name": "name",
                "value": "mark",
                "prompt": "name"
            }, {
                "name": "email",
                "value": "mark@example.com",
                "prompt": "email"
            }],
            "links": [{
                "rel": "alternate",
                "href": "http://example.com/blogs/mark",
                "prompt": "blog"
            }]
        }, {
            "href": "http://localhost:1337/muffin",
            "data": [{
                "name": "name",
                "value": "muffin",
                "prompt": "name"
            }, {
                "name": "email",
                "value": "muffin@example.com",
                "prompt": "email"
            }],
            "links": [{
                "rel": "alternate",
                "href": "http://example.com/blogs/muffin",
                "prompt": "blog"
            }]
        }],
        "queries": [{
            "rel": "collection sort",
            "prompt": "Sort by Name",
            "href": "http://localhost:1337/sortbyname"
        }, {
            "rel": "collection filter",
            "prompt": "Filter by Name",
            "href": "http://localhost:1337/filterbyname",
            "data": [{
                "name": "name",
                "value": "",
                "prompt": "Name"
            }]
        }, {
            "rel": "collection sort",
            "prompt": "Sort by Email",
            "href": "http://localhost:1337/sortbyemail"
        }],
        "template": {
            "data": [{
                "name": "name",
                "value": "",
                "prompt": "Name"
            }, {
                "name": "email",
                "value": "",
                "prompt": "Email"
            }, {
                "name": "blog",
                "value": "",
                "prompt": "Blog"
            }]
        }
    }
}
```
