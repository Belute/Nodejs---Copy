

# Select Dog Breed



This project is for **educational** porpuses only. 

Site published at: https://belute.github.io/Select_dog_breed_API/


## Project features


-   CSS
-   JS
-   html

## Authors

Justinas: [Github](https://github.com/Belute)

## Code sample

```css
#rezultatas img{
  text-align: center;
}

#rezultatas img {
  max-width:320px;
}
```

``` js

    for (let i = 0; i < objectLength; i++) {

        var option = document.createElement("option");
        var select = document.getElementById("batchSelect");
        select.appendChild(option);
        option.innerText = array[i]



        bb[i].forEach(element => {
            var option = document.createElement("option");
            var select = document.getElementById("batchSelect");
            select.appendChild(option);
            option.innerText = array[i] + "/" + element
        });

    }


})

```
```html
<main>


        <div id="rezultatas">
            <img id=img src=""></img>
        </div>

        <button id=btn class="findBreed"></button>

        </div>
        <select id="batchSelect">


        </select>

    </main>

```
