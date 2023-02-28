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
- My [ilovapples.github.io](//ilovapples.github.io) page


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
```  
```python
# | JSON_FILE_NAME ||
# | -------------- | -|
# | tag1 | val1 |
# | tag2 | val2 |
# | tag3 | val3 |
# | tag4 | val4 |


import json
def json_to_md(json_path):
  json_contents = json.loads(open(json_path).read())
  
  if isinstance(json_contents, list):
    if "/" in json_path:
      md = '# ' + json_path[json_path.rindex("/")+1:json_path.rindex('.')] + '\n'
    else:
      md = '# ' + json_path[:json_path.rindex('.')] + '\n'
    
    for index, _dict in enumerate(json_contents):
      md += f'| Num: {index} |  |\n| - | - |\n'
      for key in _dict:
        md += f'| {key} | {json_contents[index][key]} |\n'
      md += '---\n'
  else:
    for key in json_contents:
      md += f'| {key} | {json_contents[key]} |\n'
  return md
print(json_to_md("Minecraft Items.json"))
```
<br>
<br>
<br>
<br>
<br>
<br>
<br>

# Stats

## My Github Stats:
![My Github Stats](https://github-readme-stats.vercel.app/api?username=ilovapples&count_private=true)

## The number of people that have visited my profile:
![Number of people that visited my profile.](https://profile-counter.glitch.me/ilovapples/count.svg)
