# cd-express
using express through configuration

## Install

```
$ npm install cd-express
```

## Usage
```
$ cd-express --init
$ cd-express
```

### cd-express.json
```
{
    "$schema":"https://jsonschema-zh-hans.github.io/schemas/cd-express.json",
    "port":8988,
    "debug":true,
    "open":{
        
    },
    "static": { 
        "/": [ "./public" ] 
    },
    "router":{
        "/api":"./router"
    },
    "proxy":{ 
        "/":[
            {"target":"http://127.0.0.1:5009"}
        ] 
    }
}
```
