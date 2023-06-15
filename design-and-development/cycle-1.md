# 2.2.1 Cycle 1

## Design

In the first cycle I have decided to make a basic layout for a home page with very limited functionality. I have done this with a combination of HTML and CSS. I am keeping it simple as the features of this project are a priority, so any addition customisation will be handled in future cycles.

### Objectives

Create a simple home page which the user can use to navigate to the tools of this application.

* [x] Create a layout for the home page
* [x] Add simple customisation to improve user experience.

### Usability Features

A basic web page that has three interactable buttons which will take the user to three different pages. Buttons will have some css to prevent colouration when clicked

### Key Variables

| Variable Name         | Use                                    |
| --------------------- | -------------------------------------- |
| stylesheet            | apply customisation to website         |
| buttons               | categories all buttons under one class |
| portfolio\_management | specified ID for that button           |
| market\_management    | specified ID for that button           |
| wallet                | specified ID for that button           |

### Example format

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

## Development

### Outcome

By the end of this cycle I have created a basic web page that allows me to navigate between different html files. I added css to make it slightly visually pleasing. I also included a background to add a bit of flare. See below how this was done:

```css
/*setting background image*/
body {
    background-image: url('https://img.freepik.com/free-vector/gradient-stock-market-concept_23-2149166910.jpg?size=626&ext=jpg&ga=GA1.2.1453007049.1684830776&semt=ais');
    background-repeat: no-repeat;
    background-size: 100%;
    margin: 0;
}
```

Below is how a set up the buttons. I added interact-ability via an anchor tag which I also has an ID.

```html
<!--enclosing buttons in a section-->
<section class="buttons">
            <div id="button1">
                <!--Use anchor to make the buttons links to other pages--> 
                <button id="portfolio__management"><a id="portfolio_link" href="portfolio_management.html">Portfolio Management</a></button>    
            </div>
            <div id="button2">
                <button id="market__management"><a id="market_link" href="market_management.html">Market Management</a></button>  
            </div>
            <div id="button3">
                <button id="wallet"><a id="wallet_link" href="wallet.html">Wallet</a></button> 
            </div>
</section>
```

I added basic customisation to the buttons the make them more usable. I did this with css. These changes stopped the anchor link from turning purple when clicked. It also increased the clickable area for the button.

```css
/*Preventing change in colour when link clicked*/
#market_link {
    color: white;
    text-decoration: none;
}

#wallet_link {
    color: white;
    text-decoration: none;
}

#portfolio_link {
    color: white;
    text-decoration: none;
}

a {
    z-index: 1;
    padding: 2em;
    margin: -2em;
  }
```

I also added a button customisation to the size and style of the button below. This involved increasing the border and padding size to increase the size of the button.

```css
/*Adding customisation to the buttons*/
#portfolio__management {
    padding: 20px;
    margin: 50px 50px 50px 0;
    font-size: large;
    background-color: transparent;
    color: white;
}

#market__management {
    padding: 20px;
    padding-right: 29px;
    padding-left: 29;
    margin: 50px 50px 50px 0px;
    font-size: large;
    background-color: transparent;
    color: white;
}

#wallet {
    padding: 20px;
    padding-right: 80px;
    padding-left: 80px;
    margin: 50px 50px 50px 0px;
    font-size: large;
    background-color: transparent;
    color: white;
}
```

### Challenges

I experienced no real challenges with this cycle. The only main challenge was deciding what method to use to achieve certain outcomes. This involved finding the right way to make the background image cover the who page and making the buttons the same size

## Testing

{% file src="../.gitbook/assets/ocr-homepage-eveidence.mp4" %}
Testing evidence using the home page
{% endfile %}

### Tests

| Test | Instructions  | What I expect             | What actually happens | Pass/Fail |
| ---- | ------------- | ------------------------- | --------------------- | --------- |
| 1    | Run code      | Website loads up          | As expected           | Pass      |
| 2    | Press buttons | Take me to indicated page | As expected           | Pass      |
