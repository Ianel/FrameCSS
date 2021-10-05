# FrameCSS

This is a project showing some features that may be useful to integrate into some CSS frameworks like Bootstrap or TailwindCSS. The goal is to add as much features as possible in a CSS framework that would allow its users to have both flexibility and speed in the reach of some classes.

## Main Feature
Customizable parameters(margin, padding, font-size, width, height, ...) based on a bases parameters applied on the body tag. 

## Types of bases
- Base for margin and padding: `--base`
- Base for font-size: `--text-base`

## Explanations
#### Base for margins and paddings
The CSS variable `--base` defines the base parameter for the margins and the paddings. You can customize it to fit your need. For the moment, its values are `.base-4`, `.base-8` and `.base-16`. The numbers are the base values in pixels. All the calculations are based on the `--base` variable.

#### Base for font sizes
The CSS variable `--text-base` defines the base parameter for the font sizes. You can customize it to fit your need. For the moment, its values are `.text-base-4`, `.text-base-6` and `.text-base-8`. The numbers are the base values in pixels. All the calculations are based on the `--text-base` variable.

### Code sample
```html
<body class="base-16 text-base-6">
    <header>
      <img class="px-2 py-1" src="./assets/images/Logo.svg" alt="YelpCamp Banner" />
    </header>

    <main class="px-2">
        <div>
            <h1 class="text-sm font-regular">Explore the best camps on Earth.</h1>
            <p>YelpCamp is a curated list of the best camping spots
                on Earth. Unfiltered and unbiased reviews.
            </p>
            <div>
                <i class="fas fa-check-circle"></i>
                <span>Add your own camp suggestions</span>
            </div>
            <div>
                <i class="fas fa-check-circle"></i>
                <span>Leave reviews and experiences</span>
            </div>
            <div>
                <i class="fas fa-check-circle"></i>
                <span>See locations for all camps</span>
            </div>
            <button>View campgrounds</button>
        </div>
        <div>
            <img src="./assets/images/Hero Image (Tablet and Mobile).jpg" alt="Hero Image" />
        </div>
    </main>
</body>
```