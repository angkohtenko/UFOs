# UFOs
## Overview of Project
The purpose of the project was to create a webpage and dynamic table with filters using JavaScript and Bootstrap.

## Results
### Steps taken
I’ve created 3 JavaScript functions in [app.js](https://github.com/angkohtenko/UFOs/blob/main/static/js/app.js): to build table from given [dataset](https://github.com/angkohtenko/UFOs/blob/main/static/js/data.js), to get values from filters provided by user and to filter the table.

Then I’ve created the [webpage](https://github.com/angkohtenko/UFOs/blob/main/index.html) using Bootstrap and added the script to make a table dynamic.
Now user can filter the table based on 5 criteria: date, city, state, country and shape of UFO. I filled every field with a placeholder for better understanding of expected values.
I used [style.css](https://github.com/angkohtenko/UFOs/blob/main/static/css/style.css) to adjust a font color for body text and jumbotron background image.

### Output
Once user types any value to the filter and presses Enter, the table is sorted and only appropriate values are displayed. 
For example, if the table is filtered by city value “la mesa”, the result will be next:

![](https://github.com/angkohtenko/UFOs/blob/main/static/images/filtered_table_city.png)

If one more filter is added – shape is light – the output will be changed:

![](https://github.com/angkohtenko/UFOs/blob/main/static/images/filtered_table_city_shape.png)
 
## Summary
The biggest drawback of current design, in my opinion, is the similar color for a placeholder and user’s value in the filter. It’s hard to distinguish one from another. I would change the font color by editing style.css:

```
input {
    color: black !important;
}

::placeholder {
    color:lightgray !important;
}
```

Then I would add ``` class="form-control" ``` to the date filter, so all filter fields will look the same. It will make design neater.

Also, I would add tag ```</br>``` to subheading  ```<h3 />``` to split the title and put “UFO Sightings: Fact or Fancy?” and “Ufologists Weigh In” into two separate lines:
```
<h3>UFO Sightings: Fact or Fancy? <br/><small>Ufologists Weigh In</small></h3>
```

So, after all adjustments the final output will look like that:
![image](https://github.com/angkohtenko/UFOs/blob/main/static/images/adjusted_design.png)

