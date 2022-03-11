

# Dog breed



This project is for **educational** porpuses only. Pull request are welcome, but priority for project authors! Thank you for your cooperation!

Site published at: https://belute.github.io/Select_dog_breed/


## Project features


-   CSS
-   JS

## Authors

Justinas: [Github](.......)

## Code sample

```async function getBySeason() {
    const requestURL = `https://dog.ceo/api/breeds/list/all`
    const request = new Request(requestURL);
    const response = await fetch(request);
    const data = await response.json();
    console.log(data)
    return data;
}

async function getImg(breed) {
    const requestURL = `https://dog.ceo/api/breed/` + breed + `/images/random`;
    const request = new Request(requestURL);
    const response = await fetch(request);
    const data = await response.json();

    const img = document.getElementById("img")
    img.src = data.message
    console.log(data)
    return data;
}

getBySeason().then(data => {
    // console.log(data.message)
    let objectLength = Object.keys(data.message).length
    let aa = Object.values(data.message)
    const propertyNames = Object.keys(data.message);
    let array = Object.values(propertyNames)
    bb = Object.values(aa)





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


document.getElementById("btn").addEventListener('click', () => {
    let breed = document.querySelector('select').value
    console.log(breed)
    getImg(breed)
    console.log("Labas")
    console.log(breed)

})












```
