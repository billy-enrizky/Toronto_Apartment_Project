# Toronto Apartment Project

This project aims to visualize apartment building evaluation data in Toronto using the Folium library. The code provided generates an interactive map displaying the locations of apartment buildings and their corresponding evaluation scores. Here's an overview of the steps performed in the code:

1. **Setting the Map**: The Folium library is used to create a map centered around the coordinates [43.70501705, -79.41068568] with an initial zoom level of 15.

2. **Creating the 'SCORE_CLASS' Column**: A new column named 'SCORE_CLASS' is added to the apartment_data DataFrame. This column categorizes the evaluation scores into different classes ('A', 'B', 'C', 'D', 'E') based on predefined score ranges.

3. **Defining Marker Colors**: A dictionary called color_mapping is created to map each score class to a specific marker color. The color_mapping dictionary assigns black, blue, green, red, and dark red colors to classes 'A', 'B', 'C', 'D', and 'E', respectively.

4. **Adding Markers to the Map**: Iterating over the apartment_data DataFrame, markers are added to the map for each apartment location. The latitude, longitude, score class, and site address are used to position the markers and assign the corresponding marker color.

5. **Creating a Custom Legend**: A custom legend is created as an HTML div element. It displays the marker colors and their corresponding score classes.

6. **Adding the Legend to the Map**: The custom legend is added to the map using the `add_child` method of the Folium HTML object.

7. **Adding Layer Control**: A layer control is included to allow toggling the legend on and off.

The resulting map provides a visual representation of apartment building locations in Toronto, with different marker colors indicating the evaluation score classes. Users can interact with the map and explore the distribution of apartment buildings across the city.

**Note**: Make sure to replace the `apartment_data` variable with the actual DataFrame containing the apartment building evaluation data.

Feel free to customize the code according to your specific needs and data to further enhance the visualization.
