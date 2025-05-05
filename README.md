<h1>📚 Project Overview</h1>
<p>This project focuses on forecasting residential energy usage and uncovering consumption patterns by integrating home characteristics, hourly weather data, and energy consumption records.
It simulates the impact of rising summer temperatures and provides actionable insights to assist energy providers in managing peak loads and optimizing grid efficiency.</p>
<br>

<h1>🎯 Business Objective</h1>
<p>Energy companies face increasing challenges in predicting and managing electricity demand, particularly with extreme weather events becoming more frequent. The primary objectives of this project were:
  <ul>
    <li>Forecast residential energy usage during hotter-than-average summer conditions.</li>
    <li>Identify key drivers of electricity consumption across different households.</li>
    <li>Propose data-driven strategies for mitigating peak demand pressures without costly infrastructure expansion.</li>
    <li>Simulate a +5°F increase to forecast potential energy spikes.</li>
  </ul></p>

<br>
<h1>📈 Key Insights</h1>
<ul>
  <li><b>Temperature Sensitivity:</b> Energy consumption rises sharply with temperature increases, particularly for cooling systems.</li>
  <li><b>Peak Load Hours:</b> Usage consistently peaks between 3 PM to 7 PM.</li>
  <li><b>Home Characteristics:</b> Larger homes and those with additional stories show higher energy sensitivity to temperature changes.</li>
  <li><b>Forecast Results:</b> A simulated 5°C warming scenario projected a ~21% increase in average energy consumption.</li>
</ul>

 <br>
 <h1>🛠 Technologies Used</h1>
 <ul>
   <li><b>Programming Language:</b> R</li>
   <li><b>Packages:</b> arrow, caret, dplyr, e1071, ggplot2, lubridate, Metrics, purrr, quanteda, randomForest, readr, shiny, sf, tidyverse, tigris, xgboost, leaflet</li>
   <li><b>Visualization:</b> ggplot2, viridis</li>
   <li><b>App Deployment:</b> Shiny Web App</li>
 </ul>

 <br>
 <h1>🔧 Data Preprocessing</h1>
 <ul>
   <li>Loaded and merged data from multiple sources (energy, weather, static house info).</li>
   <li>Addressed missing values using methods like median imputation and NA flagging.</li>
   <li>Standardized timestamps and filtered for complete July datasets (744 hours x 5000 houses).</li>
   <li>Applied feature engineering, including hour-of-day and weekday indicators.</li>
 </ul>

 <br>
 <h1>📊 Data Visualization</h1>
 <ul>
   <li>Derived strategic insights through exploratory data analysis and advanced ggplot2 visualizations, identifying temporal, geographic, and structural drivers of peak energy demand that informed model architecture and utility planning decisions.</li>
 </ul>   

 <br>
 <h1>💻 Shiny Dashboard Features</h1>
 <p>This dashboard was developed to translate complex energy analytics into an accessible, interactive experience for non-technical users such as utility planners, energy analysts, and city administrators. Built using R and Shiny, it provides granular control over time, geography, and appliance-specific usage—allowing users to simulate real-world energy scenarios.</p>
<h4>🔌 Energy Usage by Appliance</h4>
<ul>
  <li>Filter energy consumption data by <strong>Building ID</strong>, <strong>date range</strong>, <strong>hour of the day</strong>, and <strong>specific appliances</strong> (e.g., cooling systems, refrigerators, lighting).</li>
  <li>View interactive time series plots that display usage trends by appliance and easily compare multiple energy sources with distinct color lines.</li>
  <li>Ideal for understanding how different household systems contribute to overall energy demand.</li>
</ul>
<h4>📊 Usage Statistics Panel</h4>
<ul>
  <li>Automatically generates summary statistics for selected filters, including:</li>
  <ul>
    <li><strong>Mean</strong>, <strong>Max</strong>, and <strong>Min</strong> energy usage</li>
    <li><strong>Timestamp</strong> of peak and lowest usage</li>
  </ul>
  <li>Helps users quickly grasp consumption patterns and identify extremes without needing to analyze raw data.</li>
</ul>
<h4>🗺️ County-Level Comparison</h4>
<ul>
  <li>Interactive <strong>leaflet map</strong> visualizes average energy usage across South Carolina counties.</li>
  <li>Select different energy types (e.g., Cooling or Total Energy) to highlight usage intensity by region.</li>
  <li>Color-coded heatmaps assist in identifying high-consumption areas potentially driven by local weather or home characteristics.</li>
</ul>
<h4>🔥 +5°F Predicted Usage Simulation</h4>
<ul>
  <li>Simulates the impact of a <strong>5°F temperature increase</strong> on energy demand using a trained <strong>Random Forest model</strong>.</li>
  <li>Visualizes projected energy usage over time for selected homes, allowing users to anticipate and plan for potential peak loads.</li>
</ul>
<h4>🌍 Predicted County-Level Demand Map</h4>

<br>
<h1>🔮 Future Enhancements (Project-Specific)</h1>
<ul>
  <li><strong>Add Cost Estimation:</strong> Show estimated energy bills based on usage and utility rates.</li>
  <li><strong>Cluster Homes by Usage:</strong> Group buildings into segments (e.g., low, medium, high users) for comparison.</li>
  <li><strong>API Weather Forecast Integration:</strong> Predict near-future usage using real weather forecasts (OpenWeatherMap API).</li>
  <li><strong>Model Comparison Panel:</strong> Include XGBoost or Linear Regression alongside Random Forest for benchmark accuracy.</li>
  <li><strong>Personalized Energy Tips:</strong> Display energy-saving suggestions based on a home's size, usage, and appliance trends.</li>
</ul>
<ul>
  <li>A second heatmap shows <strong>forecasted county-wise energy usage</strong> under the +5°F scenario.</li>
  <li>Enables comparison between current and predicted loads to support energy infrastructure planning and resilience strategies.</li>
</ul>

<h3>🧾 Final Project Code</h3>
<p>The complete R Markdown file for this project is now available here: <br><b>IST_687_Final_Project_Code.Rmd</b></p>
<p>This file includes:</p>
<ul>
  <li>Data cleaning, integration, and preprocessing</li>
  <li>Feature engineering and exploratory visualizations</li>
  <li>Forecast modeling using Random Forest</li>
  <li>Simulation analysis with a +5°F temperature increase</li>
  <li>Statistical summaries and insights</li>
</ul>


