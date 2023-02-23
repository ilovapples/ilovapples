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
  
# | JSON_FILE_NAME ||
# | -------------- | -|
# | tag1 | val1 |
# | tag2 | val2 |
# | tag3 | val3 |
# | tag4 | val4 |


def json_to_md(json_path):
  if "/" in json_path:
    md = '| ' + json_path[json_path.rindex("/")+1:json_path.rindex('.')] + ' ||\n| - | - |\n'
  else:
    md = '| ' + json_path[:json_path.rindex('.')] + ' ||\n| - | - |\n'
  json_contents = json.loads(open(json_path).read())
  
  for key in json_contents:
    md += f'| {key} | {json_contents[key]} |\n'
  return md
print(json_to_md("JSON_FILE_NAME.json"))
```
