# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (number){
  let table = ""

  const count = Array(10).fill(true)

  for (iteration in count) {
    let spacer = ""
    if (iteration < 10){
      spacer = "\n"
    }
    table = `${table}${iteration} * ${number} = ${iteration * number}${spacer}`
  }

  return table
}
```

| Input | Output |
| 1     | "0" * "1" = "0"
          "1" * "1" = "1"
          "2" * "1" = "2"
          "3" * "1" = "3"
          "4" * "1" = "4"
          "5" * "1" = "5"
          "6" * "1" = "6"
          "7" * "1" = "7"
          "8" * "1" = "8"
          "9" * "1" = "9" |
| 10    | "0" * "10" = "0"
          "1" * "10" = "10"
          "2" * "10" = "20"
          "3" * "10" = "30"
          "4" * "10" = "40"
          "5" * "10" = "50"
          "6" * "10" = "60"
          "7" * "10" = "70"
          "8" * "10" = "80"
          "9" * "10" = "90"| 
| 0     | "0" * "0" = "0"
          "1" * "0" = "0"
          "2" * "0" = "0"
          "3" * "0" = "0"
          "4" * "0" = "0"
          "5" * "0" = "0"
          "6" * "0" = "0"
          "7" * "0" = "0"
          "8" * "0" = "0"
          "9" * "0" = "0" | 
|  100  | "0" * "100" = "0"
          "1" * "100" = "100"
          "2" * "100" = "200"
          "3" * "100" = "300"
          "4" * "100" = "400"
          "5" * "100" = "500"
          "6" * "100" = "600"
          "7" * "100" = "700"
          "8" * "100" = "800"
          "9" * "100" = "900"| 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program takes a number as an input and returns a table of the inputted number being multiplied by numbers 0 through nine and includes each product.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
