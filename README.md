# How To Scroll Details

This repository will show you how to add a vertical *scroll bar* to the **details** of a **summary** tag.

For example, this is a typical summary/details - 

```html
<details>
    <summary>
        Here is typicall summary and details, click this to see the details.
    </summary>
    <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore.
    </p>
</details>
```

Yes, they're kinda cool and you can style them to change their appearance. But what if you want to contain the details in a constrained space?

However, to make the details content scrollable we will need some CSS - 

```css
.details-container {
  height: 5rem;
  overflow-y: scroll;
}
```

And now the HTML - 

```html
<details>
    <summary>
        The details content is height constrained and has a vertical 
        scroll bar. The text will expand and increase the height of 
        the page but not as much.
    </summary>
    <div class="details-container" style="border: 2px solid black;">
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Massa tincidunt dui ut ornare lectus sit amet est placerat. Non nisi est sit amet facilisis magna. Eget nulla facilisi etiam dignissim diam quis. At volutpat diam ut venenatis tellus in. Duis convallis convallis tellus id interdum velit. Quis enim lobortis scelerisque fermentum dui. Fermentum odio eu feugiat pretium nibh ipsum consequat. Nibh praesent tristique magna sit amet purus gravida quis blandit. Commodo nulla facilisi nullam vehicula ipsum a arcu cursus. Et sollicitudin ac orci phasellus egestas tellus rutrum tellus pellentesque. Orci nulla pellentesque dignissim enim sit amet. Fringilla est ullamcorper.
        </p>
        <p>
            <strong>Can you scroll to see me?</strong>Senectus et netus et malesuada fames. Faucibus scelerisque eleifend donec pretium vulputate sapien nec sagittis aliquam. Faucibus in ornare quam viverra orci sagittis. Sapien pellentesque habitant morbi tristique senectus et netus. <strong>Can you scroll to see me too???</strong>
        </p>
    </div>
</details>
```

All of the *lorem ipsum* is meant to be of sufficient quantity so that the scroll bar will appear. 

## Demonstration

There are two files, `index.css` and `index.html`. Minimally just drop the HTML file onto your browser.

---
<img src="http://webexperiment.info/extcounter/mdcount.php?id=scrollable-summary_details">

