# HttpLibrary
http lib used to make rest calls easily in  c# projects

# How to use
integrate the dll in working project from HttpLibrary/tree/master/ClassLibrary1/bin/Debug/ClassLibrary1.dll

# GET
```

                    HttpProperties httpProperty = new HttpProperties()
                    {
                        dictObject = null,
                        methodType = "GET",
                        sync = true,
                        token = this.token.access_token, --optional
                        url =<request url>
                    };

                    object s = Http.HttpRequest(httpProperty);
```

# POST

```
                    Dictionary<string, string> dict = new Dictionary<string, string>();
                    dict.Add("xxKey",xxxxvalue);
                    dict.Add("xxKey",xxxxvalue);
                            
                    HttpProperties httpProperty = new HttpProperties()
                    {
                        dictObject = dict,
                        methodType = "POST",
                        sync = true,
                        token = this.token.access_token, --optional
                        url =<request url>
                    };

                    object s = Http.HttpRequest(httpProperty);
```
