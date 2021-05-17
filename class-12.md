# Chart.js

It's easy to get started with Chart.js. All that's required is the script included in your page along with a single `<canvas>` node to render the chart.

## Getting Started

Let's get started using Chart.js!

1. First, we need to have a canvas in our page.

> `<canvas id="myChart" width="400" height="400"></canvas>`

2. Now that we have a canvas we can use, we need to include Chart.js in our page.

> `<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>`

3. Now, we can create a chart. We add a script to our page.

        var ctx = document.getElementById('myChart').getContext('2d');
        var myChart = new Chart(ctx, {
            type: 'bar',
            data: {
        labels: ['Red', 'Blue', 'Yellow'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
            ],
            borderWidth: 1
        }]
        },
        options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
        }
        });

# The `<canvas>` element

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height.

The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the **2D rendering context**.

![charts](https://d6vdma9166ldh.cloudfront.net/media/images/rraph.jpg)