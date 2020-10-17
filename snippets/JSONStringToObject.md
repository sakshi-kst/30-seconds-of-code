---
title: StringToJSONObject
tags: string,object,json,intermediate
---

Converts a String array to JSON object and then prints the first key- value pair

- Use `JSON.parse(jsonString)` to convert the String to JSON Object.
- Use `Object.keys(jsonObject)` to get the keys from JSON Object. Index 0 return the first key.
- Use `jsonObject[Object.keys(jsonObject)[0]]` to get the value corresponding to the first key in the converted JSON Object.
- Function returns the first key- value pair of the JSON Object.

```js
const StringToJSONObject = (jsonString) => {
  const jsonObject = JSON.parse(jsonString);
  return Object.keys(jsonObject)[0] + ' is ' + jsonObject[Object.keys(jsonObject)[0]];
}
```

```js
console.log(StringToJSONObject('{"day1": "Sunday", "day2": "Monday", "day3": "Tuesday", "day4": "Wednesday", "day5": "Thursday", "day6": "Friday", "day7": "Saturday"}')); // 'day1 is Sunday'
```
