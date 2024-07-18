# McD-self-ordering-Kiosk
Overview:
This is a multi-page GUI application built using Tkinter in Python. It simulates an ordering system for a restaurant (specifically McDonald's) where users can select items across different categories and generate a bill in PDF format.

Features:
Main Window and Navigation:

The application starts with a main window (root) containing a Notebook (ttk.Notebook) widget that holds multiple pages (ttk.Frame instances).
Each page represents different stages of the ordering process and displays various menu items.
Pages and Functionality:

Page 1 (page1): Displays a welcome message and an image. Users start the ordering process here.
Page 2 (page2): Allows users to select eating location (eat in or take out).
Page 3 (page3): Displays menu categories (Burger, Fries, etc.) with buttons to navigate to respective pages.
Page 4 to Page 8 (page4 to page8): Each page corresponds to a specific menu category (Burgers, Fries, Chicken and Fish Sandwiches, McCafe, Beverages). Users can add items to their order, and the total amount for each category is displayed.
Page 9 (page9): Displays the final bill with the total amount calculated from all categories. Users can generate a PDF of the bill here.
Navigation and Interaction:

Buttons (tk.Button) are used for navigation between pages and adding items to the order.
Notebook.select() method is used to switch between pages dynamically based on user actions.
Global variables and functions (update_sum_and_switch) manage the order totals and updates across different pages.
PDF Generation:

Users can generate a PDF bill (generate_pdf()) from page9 using ReportLab (reportlab.pdfgen).
The PDF includes details of items ordered from each category and the total amount.
Styling and Layout:

Pages are styled using background colors (bg) and labels (tk.Label) to display text and images.
Buttons and entries (tk.Entry) are used for user interaction and input.
Purpose:
The application serves as a practical example of using Tkinter for creating a multi-page GUI with navigation, user interaction, and PDF generation functionalities suitable for a restaurant ordering system.






