> **Please submit your PR in the following format after the underline below `Results` section. Don't forget to add an underline after adding your changes i.e., at the end of your `Results` section.**

## Testing Cohere Handler
**1. Testing Detect Language**

```
CREATE MODEL mindsdb.cohere_language_detector
PREDICT language
USING
  task = 'language-detection',
  column = 'text',
  engine = 'cohere',
  api_key = 'your_api_key'
```

![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/59193367-98ab-4521-aeb4-978737d719ea)


### Querying the detect language:
```
SELECT text, language
FROM mindsdb.cohere_language_detector
WHERE text = 'Здравствуй, Мир';
```

![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/7db465ef-0a95-449b-b2bd-8e638b67fb16)




**2. Testing Summarize**

```
CREATE MODEL mindsdb.cohere_text_summarization
PREDICT summary
USING
task = 'text-summarization',
column = 'text',
engine = 'cohere',
api_key = 'MY API KEY'

```
### Querying summarize:

```
SELECT text, summary
FROM mindsdb.cohere_text_summarization
WHERE text = 'The tower is 330 metres (1,083 ft) tall,[6] about the same height as an 81-storey building, and the tallest structure in Paris. Its base is square, measuring 125 metres (410 ft) on each side. During its construction, the Eiffel Tower surpassed the Washington Monument to become the tallest human-made structure in the world, a title it held for 41 years until the Chrysler Building in New York City was finished in 1930. It was the first structure in the world to surpass both the 200-metre and 300-metre mark in height. Due to the addition of a broadcasting aerial at the top of the tower in 1957, it is now taller than the Chrysler Building by 5.2 metres (17 ft). Excluding transmitters, the Eiffel Tower is the second tallest free-standing structure in France after the Millau Viaduct. The tower has three levels for visitors, with restaurants on the first and second levels.He decorated it with furniture by Jean Lachaise and invited friends such as Thomas Edison.';
```
![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/f9cdf967-7ba1-4087-84d3-8134c4df1676)



**3. Testing Generate**

```
CREATE MODEL mindsdb.cohere_text_generation
PREDICT next_text
USING
  task = 'text-generation',
  column = 'text',
  engine = 'cohere',
  api_key = 'MY API KEY'
```

### Querying Generate

```
SELECT text, next_text
FROM mindsdb.cohere_text_generation
WHERE text = 'Once upon on a time'

```
![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/3e30d94d-ad9c-4df4-8532-d44cf15ce8e5)


### Results

Drop a remark based on your observation.
- [X] Works Great 💚 (This means that all the steps were executed successfuly and the expected outputs were returned.), Improve docs to add cohere installation.
- [ ] There's a Bug 🪲 [Issue Title](URL To the Issue you created) ( This means you encountered a Bug. Please open an issue with all the relevant details with the Bug Issue Template)

---
