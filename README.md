# CS-340
How do you write programs that are maintainable, readable, and adaptable?
Throughout this course, I focused on writing code that is modular, consistent, and easy to extend. The CRUD Python module from Project One was central to this approach. By isolating all database authentication and read operations inside a single module, I created a clean separation between the dashboard logic and the MongoDB queries. This meant the dashboard could simply call functions like read() or get_rescue_data() without needing to know anything about connection strings, query syntax, or schema details.

This structure made the Project Two dashboard significantly easier to build and maintain. When I needed to adjust rescue‑category filtering or handle empty query results, I only had to update the logic in one place. The CRUD module also made the system more adaptable I could reuse it for future dashboards, analytics tools, or any application that needs structured access to MongoDB.

How do you approach a problem as a computer scientist?
My approach to this project was grounded in breaking the problem into logical components and designing each one with clear responsibilities. Grazioso Salvare’s requirements involved both data processing and user‑facing visualization, so I approached the work in layers:

Model: MongoDB database accessed through the CRUD module

View: Dash components (DataTable, dropdown, bar chart, map)

Controller: Dash callbacks that update the interface based on user input

This MVC‑style structure helped me stay organized and ensured that each part of the system had a single purpose. Compared to earlier courses, this project required more autonomy and real‑world thinking. Instead of following predefined steps, I had to interpret client requirements, design queries that matched rescue criteria, and build a dashboard that handled missing data gracefully.

In future projects, I would continue using strategies such as modular design, schema planning, and defensive programming — especially when building systems that must remain stable even when data is incomplete or inconsistent.

What do computer scientists do, and why does it matter?
Computer scientists design systems that transform raw data into meaningful, actionable information. In this project, my dashboard helps Grazioso Salvare quickly identify animals suitable for water rescue, mountain/wilderness rescue, or disaster/individual tracking. By providing interactive filtering, breed visualizations, and map integration, the dashboard supports faster, more informed decision‑making.

This work matters because organizations rely on accurate, accessible data to operate efficiently. A tool like this dashboard reduces manual searching, minimizes errors, and gives staff a clear, user‑friendly way to explore shelter data. Ultimately, computer scientists help organizations like Grazioso Salvare focus more time on their mission — training and placing rescue dogs — and less time wrestling with data.
