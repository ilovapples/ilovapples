# ilovapples
<img src="src/importapple.PNG" width="75" height="75"></img>

## Friends
- [@Devilish-Bob](//github.com/devilish-bob).

## Projects

#### Datapacks
- Float-Blocks
- Snow Mess

#### Programs
- none yet

#### Websites/Webapps
- My ilovapples.github.io page


## Programming Languages
- [Python](//python.org)
- [JavaScript](//javascript.com)
- [Swift](//swift.org)

## Web-Dev/Markup Languages
- HTML
- CSS
- [JavaScript](//javascript.com)

---
##### JSON thing
```python
import json

def get_json(jsonpath: str) -> dict:
  json_contents = open(jsonpath).read()
  
  json_contents_dict = json.loads(json_contents)
  return {"str": json_contents, "dict": json_contents_dict}
  
# Example that prints the json file:
print(get_json("example.json")["str"])
```
