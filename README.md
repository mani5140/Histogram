# The Deployed link is
https://histograms.onrender.com


# Here's how the code works:

We start by importing the necessary libraries from react, axios, react-csv, and recharts.
In the App component, we define two states using the useState hook:
data is an array that will hold the top 20 words and their count after processing the text file.
loading is a boolean that will be used to indicate if the data is being fetched or not.
We define a fetchData function that will be called when the Submit button is clicked. This function makes an HTTP GET request to the text file URL, processes the content to get the word counts, selects the top 20 words, and sets the data state with the results.
We define a csvData array that will hold the data in the format required for the CSV file. We use the map function to convert each object in data to an object with word and count properties.
In the JSX code, we render a button that calls the fetchData function when clicked. We disable the button when loading is true.
When data has a length greater than 0, we render a BarChart component from recharts with the data. We also add an h2 tag to show the title of the chart.