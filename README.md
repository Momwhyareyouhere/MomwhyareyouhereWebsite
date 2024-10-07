# MomwhyareyouhereWebsite

MomwhyareyouhereWebsite is a package that allows you to host website.

Pypi:[Pypi](<https://pypi.org/project/MomwhyareyouhereWebsite/>)

# Usage

First insert the import:
```
from mom_website import MomwhyareyouhereWebsite
```
After that put the root_directory and the port like this
```
site = MomwhyareyouhereWebsite(port=8082, root_directory="Directory")
```
Replace Directory with you real root_directory.

Now we need to make app routes like this:
```

site.add_route("/", "index.html")
site.add_route("/about", "about.html")
```

To start the server insert now:
```
site.start_server()
```

If you want to stop the server you just insert this:
```
site.stop_server()
```

Final script:
```
from mom_website import MomwhyareyouhereWebsite

site = MomwhyareyouhereWebsite(port=8082, root_directory="Directory")

site.add_route("/", "index.html")
site.add_route("/about", "about.html")

site.start_server()
```
