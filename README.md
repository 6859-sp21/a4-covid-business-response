# Business Response to the COVID-19 Pandemic (March 2020)
by Felix Dumont and Taylor Facen

### Design Decisions ###
After selecting our dataset, there were three key decisions we made with this visualization. First, we had to decide on the type of diagram. We originally planned to use a map-based visualization but then opted against this because the dataset only contains information for a subset of states and regions. The resulting map would have more empty space than filled space. We chose the sunburst diagram because its drill-down nature allows the viewer to freely dive into specific segments to uncover how different groups of businesses were prepared for conducting sales during COVID. 

The next choice was on what information to display. Because the data comes from a snapshot in time and doesn't contain how businesses changed over time, we were limited in scope in what we could portray in this visualization. However, we did have enough rich information in each business' location, category, and COVID-readiness for the static time of March 2020 which can be seen in our chart.

The last major choice was on what secondary chart should be used to complement the main sunburst diagram. Business star rating is an interesting metric that could help answer questions like "Are higher-end restaurants more likely to be COVID-ready?" or "What is the average rating of COVID-ready businesses in a southern state like Arizona versus a northern state like Pennsylvania?". A gauge chart felt like the perfect addition to display this metric. 

### An overview of your development process. 
We first sketched multiple designs by hand and met to discuss what we could potentially do. We also reviewed online D3 examples for inspiration on Observable and d3js.org.

Once we agreed on the design, we leveraged Github to share quick iterations of the graph. We split features and subcomponents (e.g. Taylor to do gauge chart, Felix to format data in JSON...) and stayed in touch frequently.

In the end, the whole process took in the order of **20-30 hours across the two of us**.

The **hardest piece** by far was to get the first iteration of the graph, as most D3 examples were in Observable and couldn't be easily leveraged. 

This proved to be a significant pain point about both Observable and D3. We also noticed that many examples used older versions of D3 and required significant work to be useable.

Agreeing on the Sunburst design also took us a significant amount of time as we initially explored other designs such as maps.