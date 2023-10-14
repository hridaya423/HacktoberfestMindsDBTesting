> **Please submit your PR in the following format after the underline below `Results` section. Don't forget to add an underline after adding your changes i.e., at the end of your `Results` section.**

## Testing Cohere Handler
**1. Testing Detect Language**

```

```



### Querying the detect language:
```

```





**2. Testing Summarize**

```
CREATE MODEL mindsdb.cohere_text_summarization
PREDICT summary
USING
task = 'text-summarization',
column = 'The tower is 330 metres (1,083 ft) tall,[6] about the same height as an 81-storey building, and the tallest structure in Paris. Its base is square, measuring 125 metres (410 ft) on each side. During its construction, the Eiffel Tower surpassed the Washington Monument to become the tallest human-made structure in the world, a title it held for 41 years until the Chrysler Building in New York City was finished in 1930. It was the first structure in the world to surpass both the 200-metre and 300-metre mark in height. Due to the addition of a broadcasting aerial at the top of the tower in 1957, it is now taller than the Chrysler Building by 5.2 metres (17 ft). Excluding transmitters, the Eiffel Tower is the second tallest free-standing structure in France after the Millau Viaduct. The tower has three levels for visitors, with restaurants on the first and second levels.He decorated it with furniture by Jean Lachaise and invited friends such as Thomas Edison.',
engine = 'cohere',
api_key = 'MY API KEY'

```


![CREATE_PREDICTOR](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/83c25ebe-8b3c-4e0b-81cf-d5bcf585f305)

**3. Testing Generate**

```
CREATE MODEL mindsdb.cohere_text_generation
PREDICT next_text
USING
  task = 'text-generation',
  column = 'Once upon a time, there was',
  engine = 'cohere',
  api_key = 'MY API KEY'
```

![image](https://github.com/hridaya423/HacktoberfestMindsDBTesting/assets/66767013/0c5dc602-7b6d-4bdc-81a4-6315ac4b7c84)



### Results

Drop a remark based on your observation.
- [X] Works Great 💚 (This means that all the steps were executed successfuly and the expected outputs were returned.), Improve docs to add cohere installation.
- [ ] There's a Bug 🪲 [Issue Title](URL To the Issue you created) ( This means you encountered a Bug. Please open an issue with all the relevant details with the Bug Issue Template)

---
