# hackaton-nvidia-skoltech

Link to figma project (Please, use "Fill - Scale down or up to fill" option for better picture):
https://www.figma.com/file/h7o4UGimhZCCEwFT9fdvE5/Untitled?node-id=0%3A1

In the repository you can find extended datasets:
* `updated_employees.csv` has additional columns with number of people managed by an employee (directly and totally), based on that we calculate radius of a node in our representation
* `employees_connections.csv` is a new artificial dataset, it represents chatting statistics of some pairs of employees (number of total messages, number of days of last two month with any messaging). Most of interactions are inside a project of an employee, but some are outside of this project. We calculate presented metric for each connection and based on that we calculate width of an edge of this connection

Refer to `extending_provided_dataset.ipynb` for Jupyter Notebook with more details on data generation

In `frontend_prototype` dericterory you may find a main page with the graph. The nodes are the employees and the size of the circle depends on the contribution of each person. At the top of the page you may see a user profile card wich suppose to appear after click on a circle. 
* `script.js` contains a graph behavior script
* `script_card.js` contains a user profile card behavior script
