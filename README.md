Page Title is not updated when publishing app, it works local debug (Release or Debug config).

My example is running on Windows, but also doesn't work in Linux Container.

# Recreate

Publish the app and run
```
dotnet publish -c Release
Server\bin\Release\net6.0\publish\HeadFail.Server.exe
```

- Open `https://localhost:5001/`, notice the page title `Hello World`.
- Click a the `Counter` link
  - *Actual* : the page title does not update.
  - *Expected*: the page title updates

Additional:
- Refresh the page, the page title updates `Counter from HeadContent`