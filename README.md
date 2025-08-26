🛠️ **MCP Leave Management Server**

A beginner-friendly MCP Server built for an HR leave management use case.
This project demonstrates how to create an MCP server, connect it with an MCP client (Claude Desktop), and handle employee leave-related operations.

-------

📌 **Features**

Check Leave Balance – Query remaining leaves for an employee.

Apply for Leave – Submit leave requests with date parsing.

View Leave History – Retrieve historical leave data for employees.

Mock Employee Database – Pre-configured with sample employees (E001, E002).

Claude Desktop Integration – Natural language interface for HR managers.

-----

⚙️ **Architecture**

  Employee Database (mock) --> MCP Server (Python) --> Claude Desktop (MCP Client) --> HR Manager (Natural Language Queries)

-----

🚀 **Getting Started**
1. Clone Repository
git clone https://github.com/d-harshini/mcp-leave-manager.git
cd mcp-leave-manager

2. Install Dependencies
pip install mcp
pip install uv
pip install typer --upgrade

3. Initialize Project
uv init my-first-mcp-server

4. Run Server
uv mcp install main.py

5. Connect with Claude Desktop

Install Claude Desktop for your OS.

Enable Developer Mode in settings.

Verify that the MCP tools (get_leave_balance, apply_leave, get_leave_history) are available.

-----

🧑‍💻 **Example Usage**

HR Manager: How many leaves does E001 have left?
Claude Desktop → Calls `get_leave_balance`
Response: E001 has 18 days remaining.

HR Manager: Apply leave for E002 on 4th July.
Claude Desktop → Calls `apply_leave`
Response: Leave applied successfully. Remaining balance: 19 days.

----

📚 **Planned Improvements**

Connect to a real employee leave database.

Support for multiple leave types (sick, vacation, personal).

Reporting and analytics features.

Integration with HR platforms.




