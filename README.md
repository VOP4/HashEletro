# HashEletro
#The project starts with creating the background for each page and tooltips were made. Created by Power Point. To know the exact size of the background, take a screenshot of the screen (Windows+SHIFT+S). The background is intended to make the analysis more intuitive for the user by containing the image of each button that will be generated in PowerBI itself. There will be three backgrounds (Cover, General and Returns). The cover has a button to take you to the "General" page.

GENERAL:
On the General page we have information on Total Revenue, Total Profit, Total Sales and Profit Margin, all this information can be filtered by dates, product category, product, location. There are three graphs and a table. A monthly revenue comparison chart year over year and adjusted to compare only the months in which there were sales. With activated tooltips for billing month information and quantity sold. The Donut Chart with the % of sales and revenue by type of store. The total revenue graph by product category has the top 5 best-selling products in the category and the total quantity sold. The graph tooltip is hidden and is one of the project pages, its design was drawn in Power Point. And a table with information on revenue, profit and total sales by continent and country, organized by hierarchy. And an interactive button to enter the page's instruction panel.

ANALYSIS:
Begin with a scroller with a month-over-month sales comparison. On this page there are several filters, the main one being "Decompsition Tree". The intention is to visualize the main parameters (sales and quantity sold) filtered by brands, type of product and the specific product, through the "Decomposition Tree".
As there would be a lot of information on the screen, I decided to separate the visualization of revenue and quantity sold, using a parameter button, I created a table that looks for the created measurements of revenue and quantity sold
Below, I used an Enlighten Data Story with the measures of best-selling product, quantity sold and % sold, using TOP N. To search for the first one, filtering by the measure of quantity sold and revenue.
The same logic and process was used in the Enlighten Story next door, but for stores and using the most sold store measure.
I added a button created on the flaticon website, it is a date filter, using the table/column "dCalendario[Datas]"
And the table/column"dLojas[Pais]".

RETURNS:
Focusing on returns, I created several measures to add up the number of products returned, through the returns column. I divided the sum value by the total number of returns to get the % returned. And I added the quantity returned by the unit value to have lost revenue.
Using the area graph, I used the %returned measure, and the column[inicio mês] from the "dcalendario" table, I activated the graph tooltip, a tooltip that was drawn in PowerPoint and the information entered in PowerBI.
A location graph containing information from the [Continente] column of the dLojas table, and the %Devoluções measure in the size of the bubbles.
And the return by brands, using the %Devoluções measure and the information from the [brand] column of the dProdutos table.

RETURN TOOLTIP:
Using the measures of %Returned, Total Returns and quantity sold. I created a chart with the TOP 5 through a filter using the quantity returned measure

SALES TOOLTIP:
Using the Total Sales and Faturamento Total measures within the card. A column chart using the Faturamento Total measure and the information from the "Nome do Produto" column of the dProduto table, filtering the TOP 5 products by the average Faturamento Total.
Simple Image to search for images from each product category. The images are from the internet. I used the imagebb website to create the URL for each image. I created the images table in Excel and took it into PowerBI with the name dImagens. I merged the dImagens table with the dProdutos table using the "Tipo de Produto" column as a reference. And using the Simple Imagem feature I placed the "Link" column that contains the url of the images generated in Imagebb as an Image Link parameter.

NOTE:
All graphs were made using measurements using table columns as a basis. Various date functions, mathematical formulas, searches in other tables. Measures that used other measurements as a basis. All with the aim of leaving the project with as few columns and tables as possible, for better optimization.
Instant Eyedropper was used to match the color tone of all pages, graphics and tooltips.
All Backgrounds were created in PowerPoint, after being designed, I selected all the fields on the slide, and saved it as a png on the computer. In the canvas background in PowerBI, I looked for the image and adjusted the PowerBI screen.
To find out the exact dimensions, I used the shortcut (windows+shift+S) to make a screenshoot and used this screenshoot as a basis for drawing in PowerPoint#
