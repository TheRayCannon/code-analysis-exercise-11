# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input | Output |
| ----- | ------------------------------------------------ |
|   3   |  { humanYears: 3, catYears: 28, dogYears: 29 }  | 
|   9   |  { humanYears: 9, catYears:52, dogYears: 59 }   | 
|   18  |  { humanYears: 18, catYears:88, dogYears: 104 } | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td> This program takes an inpout of a human age and produces the output of a calculated corresponding dog and cat age will be; Using the calculation (actualAge-2)*4+24 for cats and (actualAge-2)*5+24 for dogs, where "actualAge" is the value of human years.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
